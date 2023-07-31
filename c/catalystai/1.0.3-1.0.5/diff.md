# Comparing `tmp/catalystai-1.0.3.tar.gz` & `tmp/catalystai-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystai-1.0.3.tar", last modified: Mon Jul 31 13:50:41 2023, max compression
+gzip compressed data, was "catalystai-1.0.5.tar", last modified: Mon Jul 31 14:07:07 2023, max compression
```

## Comparing `catalystai-1.0.3.tar` & `catalystai-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 13:50:41.984546 catalystai-1.0.3/
--rw-rw-rw-   0        0        0      336 2023-07-31 13:50:31.000000 catalystai-1.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-07-31 10:18:20.000000 catalystai-1.0.3/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-07-31 10:18:20.000000 catalystai-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      543 2023-07-31 13:50:41.983546 catalystai-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-07-31 10:18:20.000000 catalystai-1.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 13:50:41.967496 catalystai-1.0.3/catalystai/
--rw-rw-rw-   0        0        0       32 2023-07-31 13:49:37.000000 catalystai-1.0.3/catalystai/__init__.py
--rw-rw-rw-   0        0        0     3316 2023-07-31 13:49:30.000000 catalystai-1.0.3/catalystai/catalystai.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:50:41.982549 catalystai-1.0.3/catalystai.egg-info/
--rw-rw-rw-   0        0        0      543 2023-07-31 13:50:41.000000 catalystai-1.0.3/catalystai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-07-31 13:50:41.000000 catalystai-1.0.3/catalystai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 13:50:41.000000 catalystai-1.0.3/catalystai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-31 13:50:41.000000 catalystai-1.0.3/catalystai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 13:50:41.985542 catalystai-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-07-31 13:50:21.000000 catalystai-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:07:07.458841 catalystai-1.0.5/
+-rw-rw-rw-   0        0        0      560 2023-07-31 14:06:57.000000 catalystai-1.0.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-07-31 10:18:20.000000 catalystai-1.0.5/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-07-31 10:18:20.000000 catalystai-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      543 2023-07-31 14:07:07.457842 catalystai-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-07-31 10:18:20.000000 catalystai-1.0.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 14:07:07.434530 catalystai-1.0.5/catalystai/
+-rw-rw-rw-   0        0        0       32 2023-07-31 13:55:47.000000 catalystai-1.0.5/catalystai/__init__.py
+-rw-rw-rw-   0        0        0     3314 2023-07-31 14:06:31.000000 catalystai-1.0.5/catalystai/catalystai.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:07:07.455837 catalystai-1.0.5/catalystai.egg-info/
+-rw-rw-rw-   0        0        0      543 2023-07-31 14:07:07.000000 catalystai-1.0.5/catalystai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-07-31 14:07:07.000000 catalystai-1.0.5/catalystai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 14:07:07.000000 catalystai-1.0.5/catalystai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-31 14:07:07.000000 catalystai-1.0.5/catalystai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 14:07:07.458841 catalystai-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-07-31 14:07:00.000000 catalystai-1.0.5/setup.py
```

### Comparing `catalystai-1.0.3/LICENCE.txt` & `catalystai-1.0.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `catalystai-1.0.3/PKG-INFO` & `catalystai-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystai
-Version: 1.0.3
+Version: 1.0.5
 Summary: Catalyst AI package
 Home-page: 
 Author: Catalyst AI
 Author-email: catalystlabs.ai@gmail.com
 License: Catalyst AI
 Keywords: python,first package
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `catalystai-1.0.3/catalystai/catalystai.py` & `catalystai-1.0.5/catalystai/catalystai.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 
 import psycopg2
 import psycopg2.extras
 from minio import Minio
 from io import BytesIO
 import pandas as pd
+import datetime
 
-class add_file:
+class Add_file:
     
     def __init__(self,email,workspace_id,project_id,data,filename):
         self.email = email
         self.workspace_id = workspace_id #202ff3a7-8644-471a-9cc0-4b882780f673
         self.project_id = project_id  #467dd3c1-2468-4b66-9aba-8072e3124582
         self.data = data
         self.filename = filename
 #         self.filetype = filetype
     
 #     @classmethod
     def add_data(self):
         user_id =  self.Validate_user()
         minio_client = self.Connect_minio()
         return_data = self.add_minio_data(minio_client,user_id)
-        splitreturndata = return_data.split("/")
-        print("Data added as {0} ".format(return_data.split("/")[len(splitreturndata)-1]))
+        splitreturndata = return_data.object_name.split("/")
+        print("Data added as {0} ".format(splitreturndata[len(splitreturndata)-1]))
         
     def Validate_user(self):
         conn = psycopg2.connect("dbname=%s user=%s host=%s password=%s" % ("postgres","master","dpg-cj29e6liuie55pg7jjk0-a.singapore-postgres.render.com","x77DG0cIoNvpd3KNmvZdqV2RK3197On1"))
         cursor = conn.cursor()
         # print("Connected to Database")
         query = "SELECT user_id from t_user where email = '%s' and is_active = true " %(self.email)
         try :
@@ -68,14 +69,14 @@
             object_name = str(self.workspace_id) +"/"+str(self.project_id)+"/data-files/"+str(current_time)+"/"+str(self.filename)
 #             print("object_name: ",object_name)
             found = minio_client.bucket_exists(str(user_id))
             if not found:
                 minio_client.make_bucket(str(user_id))
 #                 print("Bucket {} created".format(user_id))
                 result = minio_client.put_object(user_id,object_name,csv_buffer,length=-1)
-                return result.object_name
+                return result
             else:
 #                 print("Bucket {} already exists".format(user_id))
                 result = minio_client.put_object(user_id,object_name,csv_buffer,length=len(csv_bytes))
-                return result.object_name
+                return result
         except Exception as e:
             return e
```

### Comparing `catalystai-1.0.3/catalystai.egg-info/PKG-INFO` & `catalystai-1.0.5/catalystai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystai
-Version: 1.0.3
+Version: 1.0.5
 Summary: Catalyst AI package
 Home-page: 
 Author: Catalyst AI
 Author-email: catalystlabs.ai@gmail.com
 License: Catalyst AI
 Keywords: python,first package
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `catalystai-1.0.3/setup.py` & `catalystai-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 "Intended Audience :: Education",
 "Operating System :: MacOS :: MacOS X",
 "Operating System :: Microsoft :: Windows",
 "Programming Language :: Python :: 3",
 ]
 setup(
 name="catalystai",
-version="1.0.3",
+version="1.0.5",
 description="Catalyst AI package",
 long_description="Catalyst AI package to upload data to MinIO bucket",
 url="",
 author="Catalyst AI",
 author_email="catalystlabs.ai@gmail.com",
 license="Catalyst AI",
 classifiers=classifiers,
```

