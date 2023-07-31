# Comparing `tmp/shaku-database-1.1.6.tar.gz` & `tmp/shaku-database-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaku-database-1.1.6.tar", last modified: Fri Jul 21 03:37:52 2023, max compression
+gzip compressed data, was "shaku-database-1.1.7.tar", last modified: Mon Jul 31 07:34:55 2023, max compression
```

## Comparing `shaku-database-1.1.6.tar` & `shaku-database-1.1.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.296779 shaku-database-1.1.6/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.6/LICENSE
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-21 03:37:52.296441 shaku-database-1.1.6/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.6/README.md
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.284351 shaku-database-1.1.6/database/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.6/database/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.284939 shaku-database-1.1.6/database/bigquery/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.6/database/bigquery/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.6/database/bigquery/bq_sql_parser.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.6/database/bigquery/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.285319 shaku-database-1.1.6/database/cloud_sql/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.6/database/cloud_sql/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.6/database/cloud_sql/crud.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.285683 shaku-database-1.1.6/database/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:09:30.000000 shaku-database-1.1.6/database/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1580 2023-07-11 09:00:21.000000 shaku-database-1.1.6/database/cloud_storage/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.286078 shaku-database-1.1.6/gdrive_gcs_toolkit/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.6/gdrive_gcs_toolkit/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.286366 shaku-database-1.1.6/gdrive_gcs_toolkit/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.6/gdrive_gcs_toolkit/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.6/gdrive_gcs_toolkit/cloud_storage/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.286890 shaku-database-1.1.6/gdrive_gcs_toolkit/google_shared_drive/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.6/gdrive_gcs_toolkit/google_shared_drive/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)    13463 2023-07-21 03:36:50.000000 shaku-database-1.1.6/gdrive_gcs_toolkit/google_shared_drive/util.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-21 03:37:52.296854 shaku-database-1.1.6/setup.cfg
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-21 03:37:17.000000 shaku-database-1.1.6/setup.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.288020 shaku-database-1.1.6/shaku_database.egg-info/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-21 03:37:52.000000 shaku-database-1.1.6/shaku_database.egg-info/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)      666 2023-07-21 03:37:52.000000 shaku-database-1.1.6/shaku_database.egg-info/SOURCES.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-21 03:37:52.000000 shaku-database-1.1.6/shaku_database.egg-info/dependency_links.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-21 03:37:52.000000 shaku-database-1.1.6/shaku_database.egg-info/requires.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-21 03:37:52.000000 shaku-database-1.1.6/shaku_database.egg-info/top_level.txt
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.170714 shaku-database-1.1.7/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.7/LICENSE
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-31 07:34:55.170231 shaku-database-1.1.7/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.7/README.md
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.164468 shaku-database-1.1.7/database/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.7/database/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.165020 shaku-database-1.1.7/database/bigquery/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.7/database/bigquery/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.7/database/bigquery/bq_sql_parser.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.7/database/bigquery/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.165408 shaku-database-1.1.7/database/cloud_sql/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.7/database/cloud_sql/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.7/database/cloud_sql/crud.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.165770 shaku-database-1.1.7/database/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:09:30.000000 shaku-database-1.1.7/database/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1580 2023-07-11 09:00:21.000000 shaku-database-1.1.7/database/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.166033 shaku-database-1.1.7/gdrive_gcs_toolkit/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.7/gdrive_gcs_toolkit/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.166371 shaku-database-1.1.7/gdrive_gcs_toolkit/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.7/gdrive_gcs_toolkit/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.7/gdrive_gcs_toolkit/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.168373 shaku-database-1.1.7/gdrive_gcs_toolkit/google_shared_drive/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.7/gdrive_gcs_toolkit/google_shared_drive/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)    17404 2023-07-31 07:32:41.000000 shaku-database-1.1.7/gdrive_gcs_toolkit/google_shared_drive/util.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-31 07:34:55.170955 shaku-database-1.1.7/setup.cfg
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-31 07:33:01.000000 shaku-database-1.1.7/setup.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-31 07:34:55.169690 shaku-database-1.1.7/shaku_database.egg-info/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-31 07:34:55.000000 shaku-database-1.1.7/shaku_database.egg-info/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      666 2023-07-31 07:34:55.000000 shaku-database-1.1.7/shaku_database.egg-info/SOURCES.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-31 07:34:55.000000 shaku-database-1.1.7/shaku_database.egg-info/dependency_links.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-31 07:34:55.000000 shaku-database-1.1.7/shaku_database.egg-info/requires.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-31 07:34:55.000000 shaku-database-1.1.7/shaku_database.egg-info/top_level.txt
```

### Comparing `shaku-database-1.1.6/LICENSE` & `shaku-database-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.6/PKG-INFO` & `shaku-database-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.6
+Version: 1.1.7
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.6/README.md` & `shaku-database-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.6/database/bigquery/bq_sql_parser.py` & `shaku-database-1.1.7/database/bigquery/bq_sql_parser.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.6/database/bigquery/util.py` & `shaku-database-1.1.7/database/bigquery/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.6/database/cloud_sql/crud.py` & `shaku-database-1.1.7/database/cloud_sql/crud.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.6/database/cloud_storage/util.py` & `shaku-database-1.1.7/database/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.6/gdrive_gcs_toolkit/cloud_storage/util.py` & `shaku-database-1.1.7/gdrive_gcs_toolkit/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.6/gdrive_gcs_toolkit/google_shared_drive/util.py` & `shaku-database-1.1.7/gdrive_gcs_toolkit/google_shared_drive/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,21 +6,30 @@
 import pandas as pd
 import io
 from pathlib import Path
 from zipfile import ZipFile
 
 
 class GDriveToolkit:
-    def __init__(self, shared_drive_id, key_file_path):
+    def __init__(self, shared_drive_id, key_file_path, path=None):
         self.SCOPES = ['https://www.googleapis.com/auth/drive']
         self.KEY_FILE_PATH = key_file_path
         self.creds = service_account.Credentials.from_service_account_file(self.KEY_FILE_PATH, scopes=self.SCOPES)
         self.service = build('drive', 'v3', credentials=self.creds)
         self.shared_drive_id = shared_drive_id
-        self.folder_dict = self.__get_folder_hierarchy(self.shared_drive_id)
+        self.path = path
+        if self.path:
+            path_parts = Path(self.path)
+            self.root_list = [path for path in path_parts.parts]
+            if len(self.root_list) > 1:
+                self.folder_dict = self.__partial_traversal(self.shared_drive_id, self.root_list[1:])
+            else:
+                self.folder_dict = self.__full_traversal(self.shared_drive_id)
+        else:
+            self.folder_dict = self.__full_traversal(self.shared_drive_id)
 
     def __get_path_info(self, path):
 
         # get the parts of path
         path_parts = Path(path)
 
         if '.' in path_parts.name:  # Check if the last part of path is a file
@@ -29,61 +38,114 @@
         # search the corresponding file id based on the path_parts name
         current_dict = self.folder_dict
         folder_name = 'default'
         folder_id = 'default'
         path_id_name_list = {}
         for path_part in path_parts.parts[1:]:
 
-            if path_part in current_dict and "subfolders" != {}:
+            if len(current_dict[path_part].keys()) > 1:
                 folder_id = current_dict[path_part]["id"]
                 folder_name = path_part
-                current_dict = current_dict[path_part]["subfolders"]
+                current_dict = {key: value for key, value in current_dict[path_part].items() if key != 'id'}
 
 
-            elif path_part in current_dict and "subfolders" == {}:
+            else:
                 folder_id = current_dict[path_part]["id"]
                 folder_name = path_part
 
-        path_id_name_list[folder_name] = folder_id
+
+        path_id_name_list[folder_name] = {'id': folder_id}
 
         return path_id_name_list
 
-    def __get_folder_hierarchy(self, folder_id):
+    def __partial_traversal(self, folder_id, path_list):
+        if len(path_list) > 1:
+            query = f" '{folder_id}' in parents and name='{path_list[0]}' and mimeType = 'application/vnd.google-apps.folder' and trashed = false"
+            results = self.service.files().list(q=query, spaces='drive',
+                                                fields='files(id, name)',
+                                                supportsAllDrives=True,
+                                                includeItemsFromAllDrives=True,
+                                                driveId=self.shared_drive_id, corpora='drive'
+                                                ).execute()
+            items = results.get("files", [])
+            folder_dict = {
+                items[0]['name']: {
+                    'id': items[0]['id'],
+                    **self.__partial_traversal(items[0]['id'], path_list[1:])
+                }
+            }
+            return folder_dict
+        elif len(path_list) == 1 and folder_id != self.shared_drive_id:
+            query = f" '{folder_id}' in parents and name='{path_list[0]}' and mimeType = 'application/vnd.google-apps.folder' and trashed = false"
+            results = self.service.files().list(q=query, spaces='drive',
+                                                fields='files(id, name)',
+                                                supportsAllDrives=True,
+                                                includeItemsFromAllDrives=True,
+                                                driveId=self.shared_drive_id, corpora='drive'
+                                                ).execute()
+            items = results.get("files", [])
+            temp_dict = {}
+            for item in items:
+                temp_dict = self.__full_traversal(item['id'])
+            return {items[0]['name']: {'id': items[0]['id'], **temp_dict}}
+        else:
+            query = f" name = '{path_list[0]}' and mimeType = 'application/vnd.google-apps.folder' and trashed = false"
+            results = self.service.files().list(q=query, spaces='drive',
+                                                fields='files(id, name)',
+                                                supportsAllDrives=True,
+                                                includeItemsFromAllDrives=True,
+                                                driveId=self.shared_drive_id, corpora='drive'
+                                                ).execute()
+            items = results.get("files", [])
+            folder_id = items[0]['id']
+            query = f" '{folder_id}' in parents and mimeType = 'application/vnd.google-apps.folder' and trashed = false"
+            results = self.service.files().list(q=query, spaces='drive',
+                                                fields='files(id, name)',
+                                                supportsAllDrives=True,
+                                                includeItemsFromAllDrives=True,
+                                                driveId=self.shared_drive_id, corpora='drive'
+                                                ).execute()
+            items = results.get("files", [])
+            temp_dict = {}
+            for item in items:
+                temp_dict = self.__full_traversal(item['id'])
+            return {items[0]['name']: {'id': items[0]['id'], **temp_dict}}
+
+    def __full_traversal(self, folder_id):
 
         query = f" '{folder_id}' in parents and mimeType = 'application/vnd.google-apps.folder' and trashed = false"
         results = self.service.files().list(q=query, spaces='drive',
                                             fields='files(id, name)',
                                             supportsAllDrives=True,
                                             includeItemsFromAllDrives=True,
                                             driveId=self.shared_drive_id, corpora='drive'
                                             ).execute()
 
         items = results.get("files", [])
         folder_dict = {}
         for item in items:
             folder_id = item['id']
             folder_name = item['name']
-            subfolder_dict = self.__get_folder_hierarchy(folder_id)
+            subfolder_dict = self.__full_traversal(folder_id)
             if subfolder_dict != {}:
-
-                folder_dict[folder_name] = {'id': folder_id, 'subfolders': subfolder_dict}
+                folder_dict[folder_name] = {'id': folder_id, **subfolder_dict}
             else:
-                folder_dict[folder_name] = {'id': folder_id, 'subfolders': {}}
+                folder_dict[folder_name] = {'id': folder_id}
         return folder_dict
 
     def read_folder_files(self, path):
 
         # input the path and return the file name and file id
         folder_info = self.__get_path_info(path)
 
         path_parts = Path(path)
 
         folder_name = path_parts.name
 
-        folder_id = folder_info[folder_name]
+        folder_id = folder_info[folder_name]['id']
 
         try:
 
             query = f" '{folder_id}' in parents and mimeType != 'application/vnd.google-apps.folder' and trashed = false"
             results = self.service.files().list(q=query, spaces='drive',
                                                 fields='files(id, name)',
                                                 supportsAllDrives=True,
@@ -126,15 +188,15 @@
         dataframes = self.__file_loader(file_name, folder_id)
         for key in dataframes.keys():
             if file_name in key:
                 file = dataframes[key]
         return file
 
     def __file_loader(self, file_name, folder_id):
-        print("read files start")
+        print(f"start read: {file_name}")
 
         try:
 
             query = f"name = '{file_name}' and '{folder_id}' in parents and trashed = false"
             results = self.service.files().list(q=query, spaces='drive',
                                                 fields='files(id, name)',
                                                 supportsAllDrives=True,
@@ -206,35 +268,35 @@
 
         old_folder_name = old_path_parts.name
         new_folder_name = new_path_parts.name
 
         old_path_info = self.__get_path_info(old_path)
         new_path_info = self.__get_path_info(new_path)
 
-        old_folder_id = old_path_info[old_folder_name]
-        new_folder_id = new_path_info[new_folder_name]
+        old_folder_id = old_path_info[old_folder_name]['id']
+        new_folder_id = new_path_info[new_folder_name]['id']
 
-        print("moving function start")
+        print(f"start moving file {file_name} to {new_path}")
         try:
             query = f" name = '{file_name}' and '{old_folder_id}' in parents and trashed = false"
             results = self.service.files().list(q=query, fields='files(id, name)',
                                                 supportsAllDrives=True,
                                                 includeItemsFromAllDrives=True,
                                                 driveId=self.shared_drive_id, corpora='drive').execute()
-            item = results.get('files', [])
+            items = results.get('files', [])
 
-            file_id = item[0]['id']
+            file_id = items[0]['id']
 
             print(f"Moving file: {file_name}")
 
             self.service.files().update(fileId=file_id,
                                         addParents=new_folder_id,
                                         removeParents=old_folder_id,
                                         fields="id,parents", supportsAllDrives=True).execute()
-            print(f"Successfully moved file {file_name} to {new_path}")
+            print(f"successfully moved file {file_name} to {new_path}")
         except HttpError as error:
             raise f'An error occurred:{error}'
         except Exception as e:
             raise f'An error occurred:{e}'
 
     def save_to_drive(self, df, file_name, path):
 
@@ -308,33 +370,35 @@
             raise f'An error occurred:{e}'
 
     def __check_folder_exist(self, path):
 
         current_dict = self.folder_dict
         path_parts = Path(path)
         flag = False
+        path_id = None
 
         for path_part in path_parts.parts[1:]:
 
             if path_part in current_dict:
-                parent_id = current_dict[path_part]['id']
-                if current_dict[path_part]["subfolders"]:
-                    current_dict = current_dict[path_part]["subfolders"]
+                if len(current_dict[path_part].keys()) > 1:
+                    path_id = current_dict[path_part]['id']
+                    current_dict = {key: value for key, value in current_dict[path_part].items() if key != 'id'}
+
             else:
                 flag = True
+                parent_id = path_id or current_dict['id']
                 file_metadata = {
                     "name": path_part,
                     'mimeType': 'application/vnd.google-apps.folder',
                     'parents': [parent_id]
                 }
                 try:
                     new_folder = self.service.files().create(body=file_metadata, fields="id",
                                                              supportsAllDrives=True).execute()
-                    current_dict[path_part] = {"id": new_folder['id'], "subfolders": {}}
-                    parent_id = new_folder['id']
+                    current_dict[path_part] = {"id": new_folder['id']}
+                    print(f"folder {path_part} is not existed and has been created.")
                 except HttpError as error:
                     raise f'An error occurred:{error}'
 
-        if flag == True:
-            self.folder_dict = self.__get_folder_hierarchy(self.shared_drive_id)
+        if flag:
+            self.folder_dict = self.__partial_traversal(self.shared_drive_id, self.root_list)
             print("some folders are not existed and have been created.")
-
```

### Comparing `shaku-database-1.1.6/setup.py` & `shaku-database-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 HERE = pathlib.Path(__file__).parent.resolve()
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 EX_INSTALL_REQUIRES = {s.strip().split('==')[0]: s.strip().split('==')[1] if len(s.strip().split('==')) > 1 else ""
                        for s in requirements.split("\n")}
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
 setup(
     name="shaku-database",
-    version="1.1.6",
+    version="1.1.7",
     author="hawktorng",
     author_email="hawktorng@shaku.com.tw",
     description="Shaku Database util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/hawktorng1/test_shaku",
     packages=find_packages(),
```

### Comparing `shaku-database-1.1.6/shaku_database.egg-info/PKG-INFO` & `shaku-database-1.1.7/shaku_database.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.6
+Version: 1.1.7
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.6/shaku_database.egg-info/SOURCES.txt` & `shaku-database-1.1.7/shaku_database.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.6/shaku_database.egg-info/requires.txt` & `shaku-database-1.1.7/shaku_database.egg-info/requires.txt`

 * *Files identical despite different names*

