# Comparing `tmp/mongodb_python_manager-1.5.6.tar.gz` & `tmp/mongodb_python_manager-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_python_manager-1.5.6.tar", max compression
+gzip compressed data, was "mongodb_python_manager-1.5.7.tar", max compression
```

## Comparing `mongodb_python_manager-1.5.6.tar` & `mongodb_python_manager-1.5.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1080 2023-07-27 09:59:52.406521 mongodb_python_manager-1.5.6/LICENSE
--rw-r--r--   0        0        0     5051 2023-07-27 09:59:52.406740 mongodb_python_manager-1.5.6/README.md
--rw-r--r--   0        0        0     9790 2023-07-27 09:59:52.407019 mongodb_python_manager-1.5.6/mongodb_python_manager/__init__.py
--rw-r--r--   0        0        0      779 2023-07-27 10:46:43.960446 mongodb_python_manager-1.5.6/pyproject.toml
--rw-r--r--   0        0        0     6037 1970-01-01 00:00:00.000000 mongodb_python_manager-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-27 09:59:52.406521 mongodb_python_manager-1.5.7/LICENSE
+-rw-r--r--   0        0        0     5051 2023-07-27 09:59:52.406740 mongodb_python_manager-1.5.7/README.md
+-rw-r--r--   0        0        0     9932 2023-07-31 09:01:48.866238 mongodb_python_manager-1.5.7/mongodb_python_manager/__init__.py
+-rw-r--r--   0        0        0      779 2023-07-31 09:02:57.444207 mongodb_python_manager-1.5.7/pyproject.toml
+-rw-r--r--   0        0        0     6037 1970-01-01 00:00:00.000000 mongodb_python_manager-1.5.7/PKG-INFO
```

### Comparing `mongodb_python_manager-1.5.6/LICENSE` & `mongodb_python_manager-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodb_python_manager-1.5.6/README.md` & `mongodb_python_manager-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_python_manager-1.5.6/mongodb_python_manager/__init__.py` & `mongodb_python_manager-1.5.7/mongodb_python_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             raise ValueError("MongoDB user and password are not set")
 
         self.uri = f"mongodb+srv://{mongo_db_user}:{mongo_db_password}@{mongo_db_cluster}/{mongodb_db_name}?retryWrites=true&w=majority"
         self.mongodb_db_name = mongodb_db_name
         self.mongodb_collection_name = None
     
     def __version__(self):
-        return "1.5.5"
+        return "1.5.6"
 
     def get_client(self) -> tuple((pymongo.MongoClient, str)):
         """
         Get client to MongoDB
         """
         client = pymongo.MongoClient(
             self.uri,
@@ -82,14 +82,20 @@
         return self.uri
 
     def get_db_name(self):
         """
         Get MongoDB database name
         """
         return self.mongodb_db_name
+    
+    def get_db(self):
+        """
+        Get MongoDB database
+        """
+        return self.client.get_database(self.mongodb_db_name)
 
     def get_collection_name(self) -> str:
         """
         Get MongoDB collection name
         """
         if self.mongodb_collection_name is None:
             raise ValueError("Collection name is not set")
```

### Comparing `mongodb_python_manager-1.5.6/pyproject.toml` & `mongodb_python_manager-1.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mongodb-python-manager"
-version = "1.5.6"
+version = "1.5.7"
 description = "The `MongoDBManager` class is a wrapper around the `pymongo` package, designed to simplify the usage of MongoDB in Python applications. It provides convenient methods for connecting to a MongoDB cluster, accessing a specific database and collection, and performing common CRUD operations."
 authors = ["louis_giron <louis@giron-dom.eu>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "mongodb_python_manager"}]
 
 [tool.poetry.dependencies]
```

### Comparing `mongodb_python_manager-1.5.6/PKG-INFO` & `mongodb_python_manager-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodb-python-manager
-Version: 1.5.6
+Version: 1.5.7
 Summary: The `MongoDBManager` class is a wrapper around the `pymongo` package, designed to simplify the usage of MongoDB in Python applications. It provides convenient methods for connecting to a MongoDB cluster, accessing a specific database and collection, and performing common CRUD operations.
 License: MIT
 Author: louis_giron
 Author-email: louis@giron-dom.eu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

