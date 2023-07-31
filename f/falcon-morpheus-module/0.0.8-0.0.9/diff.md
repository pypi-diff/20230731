# Comparing `tmp/falcon_morpheus_module-0.0.8.tar.gz` & `tmp/falcon_morpheus_module-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_morpheus_module-0.0.8.tar", max compression
+gzip compressed data, was "falcon_morpheus_module-0.0.9.tar", max compression
```

## Comparing `falcon_morpheus_module-0.0.8.tar` & `falcon_morpheus_module-0.0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     6251 2023-07-28 14:56:36.924097 falcon_morpheus_module-0.0.8/README.md
--rw-r--r--   0        0        0       61 2023-07-28 14:56:36.924097 falcon_morpheus_module-0.0.8/falcon_morpheus_module/__init__.py
--rw-r--r--   0        0        0     7314 2023-07-28 14:56:36.924097 falcon_morpheus_module-0.0.8/falcon_morpheus_module/dock_sftp_api.py
--rw-r--r--   0        0        0      325 2023-07-28 14:56:36.924097 falcon_morpheus_module-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6755 1970-01-01 00:00:00.000000 falcon_morpheus_module-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6251 2023-07-31 18:06:42.175545 falcon_morpheus_module-0.0.9/README.md
+-rw-r--r--   0        0        0       61 2023-07-31 18:06:42.175545 falcon_morpheus_module-0.0.9/falcon_morpheus_module/__init__.py
+-rw-r--r--   0        0        0     7354 2023-07-31 18:06:42.175545 falcon_morpheus_module-0.0.9/falcon_morpheus_module/dock_sftp_api.py
+-rw-r--r--   0        0        0      324 2023-07-31 18:06:42.175545 falcon_morpheus_module-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6748 1970-01-01 00:00:00.000000 falcon_morpheus_module-0.0.9/PKG-INFO
```

### Comparing `falcon_morpheus_module-0.0.8/README.md` & `falcon_morpheus_module-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `falcon_morpheus_module-0.0.8/falcon_morpheus_module/dock_sftp_api.py` & `falcon_morpheus_module-0.0.9/falcon_morpheus_module/dock_sftp_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,15 @@
             {{
                 list {{
                     { ' '.join(column_names) }
                 }}
             }}
         }}"""
 
+        print("Query : ", query_string)
         response = requests.request(
             "POST",
             url=self.morpheus_url + "/v1/query",
             headers={
                 "Authorization": f"Bearer {self.token}",
             },
             json={
```

### Comparing `falcon_morpheus_module-0.0.8/PKG-INFO` & `falcon_morpheus_module-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: falcon-morpheus-module
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: NG.CASH
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (==2.31.0)
 Description-Content-Type: text/markdown
 
 # falcon_morpheus_module
 
 
 
 ## Getting started
```

