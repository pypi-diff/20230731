# Comparing `tmp/remotion_lambda-4.0.10.tar.gz` & `tmp/remotion_lambda-4.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotion_lambda-4.0.10.tar", last modified: Tue Jul 25 00:58:21 2023, max compression
+gzip compressed data, was "remotion_lambda-4.0.14.tar", last modified: Mon Jul 31 14:22:10 2023, max compression
```

## Comparing `remotion_lambda-4.0.10.tar` & `remotion_lambda-4.0.14.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:58:21.787713 remotion_lambda-4.0.10/
--rw-r--r--   0 codedev    (503) staff       (20)     2512 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/LICENSE
--rw-r--r--   0 codedev    (503) staff       (20)      316 2023-07-25 00:58:21.787545 remotion_lambda-4.0.10/PKG-INFO
--rw-r--r--   0 codedev    (503) staff       (20)       26 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/README.md
-drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:58:21.786093 remotion_lambda-4.0.10/remotion_lambda/
--rw-r--r--   0 codedev    (503) staff       (20)      202 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/remotion_lambda/__init__.py
--rw-r--r--   0 codedev    (503) staff       (20)     5252 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/remotion_lambda/models.py
--rw-r--r--   0 codedev    (503) staff       (20)     6182 2023-07-23 00:48:40.000000 remotion_lambda-4.0.10/remotion_lambda/remotionclient.py
--rw-r--r--   0 codedev    (503) staff       (20)       85 2023-07-25 00:58:16.000000 remotion_lambda-4.0.10/remotion_lambda/version.py
-drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:58:21.786610 remotion_lambda-4.0.10/remotion_lambda.egg-info/
--rw-r--r--   0 codedev    (503) staff       (20)      316 2023-07-25 00:58:21.000000 remotion_lambda-4.0.10/remotion_lambda.egg-info/PKG-INFO
--rw-r--r--   0 codedev    (503) staff       (20)      384 2023-07-25 00:58:21.000000 remotion_lambda-4.0.10/remotion_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 codedev    (503) staff       (20)        1 2023-07-25 00:58:21.000000 remotion_lambda-4.0.10/remotion_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 codedev    (503) staff       (20)       42 2023-07-25 00:58:21.000000 remotion_lambda-4.0.10/remotion_lambda.egg-info/top_level.txt
--rw-r--r--   0 codedev    (503) staff       (20)       38 2023-07-25 00:58:21.787756 remotion_lambda-4.0.10/setup.cfg
--rw-r--r--   0 codedev    (503) staff       (20)      684 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/setup.py
-drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:58:21.787180 remotion_lambda-4.0.10/tests/
--rw-r--r--   0 codedev    (503) staff       (20)      131 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/tests/__init__.py
--rw-r--r--   0 codedev    (503) staff       (20)      474 2023-07-21 22:55:58.000000 remotion_lambda-4.0.10/tests/test_get_render_progress_client.py
--rw-r--r--   0 codedev    (503) staff       (20)      764 2023-07-21 22:55:55.000000 remotion_lambda-4.0.10/tests/test_render_client.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-07-31 14:22:10.391688 remotion_lambda-4.0.14/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     2512 2023-07-31 12:47:33.000000 remotion_lambda-4.0.14/LICENSE
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      391 2023-07-31 14:22:10.391490 remotion_lambda-4.0.14/PKG-INFO
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       26 2023-07-31 12:47:33.000000 remotion_lambda-4.0.14/README.md
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-07-31 14:22:10.388298 remotion_lambda-4.0.14/remotion_lambda/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      202 2023-07-31 12:47:33.000000 remotion_lambda-4.0.14/remotion_lambda/__init__.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     5252 2023-07-31 13:42:06.000000 remotion_lambda-4.0.14/remotion_lambda/models.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     6064 2023-07-31 14:14:39.000000 remotion_lambda-4.0.14/remotion_lambda/remotionclient.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       84 2023-07-31 13:27:17.000000 remotion_lambda-4.0.14/remotion_lambda/version.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-07-31 14:22:10.390027 remotion_lambda-4.0.14/remotion_lambda.egg-info/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      391 2023-07-31 14:22:10.000000 remotion_lambda-4.0.14/remotion_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      384 2023-07-31 14:22:10.000000 remotion_lambda-4.0.14/remotion_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)        1 2023-07-31 14:22:10.000000 remotion_lambda-4.0.14/remotion_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-07-31 14:22:10.000000 remotion_lambda-4.0.14/remotion_lambda.egg-info/top_level.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-07-31 14:22:10.391730 remotion_lambda-4.0.14/setup.cfg
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      753 2023-07-31 12:47:33.000000 remotion_lambda-4.0.14/setup.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-07-31 14:22:10.390959 remotion_lambda-4.0.14/tests/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      131 2023-07-31 12:47:33.000000 remotion_lambda-4.0.14/tests/__init__.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      474 2023-07-31 12:47:33.000000 remotion_lambda-4.0.14/tests/test_get_render_progress_client.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      764 2023-07-31 12:47:33.000000 remotion_lambda-4.0.14/tests/test_render_client.py
```

### Comparing `remotion_lambda-4.0.10/LICENSE` & `remotion_lambda-4.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.10/remotion_lambda/models.py` & `remotion_lambda-4.0.14/remotion_lambda/models.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.10/remotion_lambda/remotionclient.py` & `remotion_lambda-4.0.14/remotion_lambda/remotionclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,30 +68,28 @@
                                 aws_access_key_id=self.access_key,
                                 aws_secret_access_key=self.secret_key,
                                 region_name=self.region)
 
         return boto3.client('lambda',  region_name=self.region)
 
     def _invoke_lambda(self, function_name, payload):
-        try:
-            client = self._create_lambda_client()
-            response = client.invoke(
-                FunctionName=function_name, Payload=payload)
-            result = response['Payload'].read().decode('utf-8')
-            decoded_result = json.loads(result)
-            if 'errorMessage' in decoded_result:
-                raise ValueError(decoded_result['errorMessage'])
-            if decoded_result['statusCode'] != 200:
-                raise ValueError('Failed to invoke Lambda function')
-            body_object = json.loads(decoded_result['body'])
-            return body_object
-
-        except Exception as error:
-            print(f"Failed to invoke Lambda function: {str(error)}")
-            return None  # or you can return a default value if appropriate
+        client = self._create_lambda_client()
+        response = client.invoke(
+            FunctionName=function_name, Payload=payload)
+        result = response['Payload'].read().decode('utf-8')
+        decoded_result = json.loads(result)
+        if 'errorMessage' in decoded_result:
+            raise ValueError(decoded_result['errorMessage'])
+
+        if 'type' in decoded_result and decoded_result['type'] == 'error':
+            raise ValueError(decoded_result['message'])
+        if not 'type' in decoded_result or decoded_result['type'] != 'success':
+            raise ValueError(result)
+
+        return decoded_result
 
     def construct_render_request(self, render_params: RenderParams) -> str:
         """
         Construct a render request in JSON format.
 
         Args:
             render_params (RenderParams): Render parameters.
@@ -137,15 +135,15 @@
         Returns:
             RenderResponse: Response from the render operation.
         """
         params = self.construct_render_request(render_params)
         body_object = self._invoke_lambda(
             function_name=self.function_name, payload=params)
         if body_object:
-            return RenderResponse(**body_object)
+            return RenderResponse(body_object['bucketName'], body_object['renderId'])
 
         return None
 
     def get_render_progress(self, render_id: str, bucket_name: str) -> RenderProgress:
         """
         Get the progress of a render.
```

### Comparing `remotion_lambda-4.0.10/setup.py` & `remotion_lambda-4.0.14/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,14 @@
     author_email="jonny@remotion.dev",
     description="Remotion Lambda client",
     long_description_content_type="text/markdown",
     url="https://github.com/remotion-dev/remotion/tree/main/packages/lambda-python",
     classifiers=[
 
     ],
-    long_description="",
+    long_description="Remotion is a framework for creating videos programmatically using React.",
     packages=setuptools.find_packages(),
     python_requires='>=3.6',
     # Name of the python package
-    py_modules=["remotion-lambda-sdk"],
+    py_modules=["remotion-lambda"],
 
 )
```

### Comparing `remotion_lambda-4.0.10/tests/test_render_client.py` & `remotion_lambda-4.0.14/tests/test_render_client.py`

 * *Files identical despite different names*

