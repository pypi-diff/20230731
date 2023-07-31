# Comparing `tmp/catalystai-1.0.5.tar.gz` & `tmp/catalystai-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystai-1.0.5.tar", last modified: Mon Jul 31 14:07:07 2023, max compression
+gzip compressed data, was "catalystai-1.0.6.tar", last modified: Mon Jul 31 14:19:37 2023, max compression
```

## Comparing `catalystai-1.0.5.tar` & `catalystai-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 14:07:07.458841 catalystai-1.0.5/
--rw-rw-rw-   0        0        0      560 2023-07-31 14:06:57.000000 catalystai-1.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-07-31 10:18:20.000000 catalystai-1.0.5/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-07-31 10:18:20.000000 catalystai-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      543 2023-07-31 14:07:07.457842 catalystai-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-07-31 10:18:20.000000 catalystai-1.0.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 14:07:07.434530 catalystai-1.0.5/catalystai/
--rw-rw-rw-   0        0        0       32 2023-07-31 13:55:47.000000 catalystai-1.0.5/catalystai/__init__.py
--rw-rw-rw-   0        0        0     3314 2023-07-31 14:06:31.000000 catalystai-1.0.5/catalystai/catalystai.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:07:07.455837 catalystai-1.0.5/catalystai.egg-info/
--rw-rw-rw-   0        0        0      543 2023-07-31 14:07:07.000000 catalystai-1.0.5/catalystai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-07-31 14:07:07.000000 catalystai-1.0.5/catalystai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 14:07:07.000000 catalystai-1.0.5/catalystai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-31 14:07:07.000000 catalystai-1.0.5/catalystai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 14:07:07.458841 catalystai-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-07-31 14:07:00.000000 catalystai-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:19:37.860704 catalystai-1.0.6/
+-rw-rw-rw-   0        0        0      560 2023-07-31 14:06:57.000000 catalystai-1.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-07-31 10:18:20.000000 catalystai-1.0.6/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-07-31 10:18:20.000000 catalystai-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      543 2023-07-31 14:19:37.859702 catalystai-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-07-31 10:18:20.000000 catalystai-1.0.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 14:19:37.843706 catalystai-1.0.6/catalystai/
+-rw-rw-rw-   0        0        0       32 2023-07-31 13:55:47.000000 catalystai-1.0.6/catalystai/__init__.py
+-rw-rw-rw-   0        0        0     3352 2023-07-31 14:19:09.000000 catalystai-1.0.6/catalystai/catalystai.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:19:37.857698 catalystai-1.0.6/catalystai.egg-info/
+-rw-rw-rw-   0        0        0      543 2023-07-31 14:19:37.000000 catalystai-1.0.6/catalystai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-07-31 14:19:37.000000 catalystai-1.0.6/catalystai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 14:19:37.000000 catalystai-1.0.6/catalystai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-31 14:19:37.000000 catalystai-1.0.6/catalystai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 14:19:37.861708 catalystai-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-07-31 14:19:34.000000 catalystai-1.0.6/setup.py
```

### Comparing `catalystai-1.0.5/CHANGELOG.txt` & `catalystai-1.0.6/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `catalystai-1.0.5/LICENCE.txt` & `catalystai-1.0.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `catalystai-1.0.5/PKG-INFO` & `catalystai-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystai
-Version: 1.0.5
+Version: 1.0.6
 Summary: Catalyst AI package
 Home-page: 
 Author: Catalyst AI
 Author-email: catalystlabs.ai@gmail.com
 License: Catalyst AI
 Keywords: python,first package
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `catalystai-1.0.5/catalystai/catalystai.py` & `catalystai-1.0.6/catalystai/catalystai.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,20 +63,24 @@
     def add_minio_data(self,minio_client,user_id):
         try:
             
             csv_bytes = self.data.to_csv().encode('utf-8')
             csv_buffer = BytesIO(csv_bytes)
             current_time = datetime.datetime.now().strftime('%Y%m%d%H%M%S')
             object_name = str(self.workspace_id) +"/"+str(self.project_id)+"/data-files/"+str(current_time)+"/"+str(self.filename)
-#             print("object_name: ",object_name)
             found = minio_client.bucket_exists(str(user_id))
             if not found:
-                minio_client.make_bucket(str(user_id))
-#                 print("Bucket {} created".format(user_id))
-                result = minio_client.put_object(user_id,object_name,csv_buffer,length=-1)
-                return result
+                try :
+                    minio_client.make_bucket(str(user_id))
+                    result = minio_client.put_object(user_id,object_name,csv_buffer,length=-1)
+                    return result
+                except Exception as e:
+                    return e
+            
             else:
-#                 print("Bucket {} already exists".format(user_id))
-                result = minio_client.put_object(user_id,object_name,csv_buffer,length=len(csv_bytes))
-                return result
+                try:
+                    result = minio_client.put_object(user_id,object_name,csv_buffer,length=len(csv_bytes))
+                    return result
+                except Exception as e:
+                    return e
         except Exception as e:
             return e
```

### Comparing `catalystai-1.0.5/catalystai.egg-info/PKG-INFO` & `catalystai-1.0.6/catalystai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystai
-Version: 1.0.5
+Version: 1.0.6
 Summary: Catalyst AI package
 Home-page: 
 Author: Catalyst AI
 Author-email: catalystlabs.ai@gmail.com
 License: Catalyst AI
 Keywords: python,first package
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `catalystai-1.0.5/setup.py` & `catalystai-1.0.6/setup.py`

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
-version="1.0.5",
+version="1.0.6",
 description="Catalyst AI package",
 long_description="Catalyst AI package to upload data to MinIO bucket",
 url="",
 author="Catalyst AI",
 author_email="catalystlabs.ai@gmail.com",
 license="Catalyst AI",
 classifiers=classifiers,
```

