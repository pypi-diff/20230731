# Comparing `tmp/macaquedb-1.0.0.tar.gz` & `tmp/macaquedb-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macaquedb-1.0.0.tar", last modified: Fri Jul 21 18:24:27 2023, max compression
+gzip compressed data, was "macaquedb-1.0.1.tar", last modified: Mon Jul 31 17:08:00 2023, max compression
```

## Comparing `macaquedb-1.0.0.tar` & `macaquedb-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 18:24:27.910779 macaquedb-1.0.0/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      223 2023-07-21 18:24:27.910623 macaquedb-1.0.0/PKG-INFO
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 18:24:27.909038 macaquedb-1.0.0/macaquedb/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)    12366 2023-07-21 17:53:50.000000 macaquedb-1.0.0/macaquedb/Database.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       31 2023-07-21 17:03:41.000000 macaquedb-1.0.0/macaquedb/__init__.py
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 18:24:27.910435 macaquedb-1.0.0/macaquedb/database/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      489 2023-07-21 14:36:48.000000 macaquedb-1.0.0/macaquedb/database/Image.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      306 2023-07-21 14:36:48.000000 macaquedb-1.0.0/macaquedb/database/Session.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      321 2023-07-21 14:36:48.000000 macaquedb-1.0.0/macaquedb/database/Subject.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 16:58:35.000000 macaquedb-1.0.0/macaquedb/database/__init__.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      451 2023-07-21 14:36:48.000000 macaquedb-1.0.0/macaquedb/database/utilities.py
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 18:24:27.909835 macaquedb-1.0.0/macaquedb.egg-info/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      223 2023-07-21 18:24:27.000000 macaquedb-1.0.0/macaquedb.egg-info/PKG-INFO
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      367 2023-07-21 18:24:27.000000 macaquedb-1.0.0/macaquedb.egg-info/SOURCES.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        1 2023-07-21 18:24:27.000000 macaquedb-1.0.0/macaquedb.egg-info/dependency_links.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       14 2023-07-21 18:24:27.000000 macaquedb-1.0.0/macaquedb.egg-info/requires.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       10 2023-07-21 18:24:27.000000 macaquedb-1.0.0/macaquedb.egg-info/top_level.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       38 2023-07-21 18:24:27.910832 macaquedb-1.0.0/setup.cfg
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      372 2023-07-21 18:23:55.000000 macaquedb-1.0.0/setup.py
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 17:08:00.438461 macaquedb-1.0.1/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      268 2023-07-31 17:08:00.438324 macaquedb-1.0.1/PKG-INFO
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)     2335 2023-07-28 16:05:19.000000 macaquedb-1.0.1/README.md
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 17:08:00.435897 macaquedb-1.0.1/macaquedb/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)    16717 2023-07-31 17:01:29.000000 macaquedb-1.0.1/macaquedb/Database.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       31 2023-07-21 17:03:41.000000 macaquedb-1.0.1/macaquedb/__init__.py
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 17:08:00.437996 macaquedb-1.0.1/macaquedb/database/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      489 2023-07-21 14:36:48.000000 macaquedb-1.0.1/macaquedb/database/Image.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      306 2023-07-21 14:36:48.000000 macaquedb-1.0.1/macaquedb/database/Session.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      294 2023-07-31 15:08:30.000000 macaquedb-1.0.1/macaquedb/database/Subject.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 16:58:35.000000 macaquedb-1.0.1/macaquedb/database/__init__.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      451 2023-07-21 14:36:48.000000 macaquedb-1.0.1/macaquedb/database/utilities.py
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 17:08:00.436911 macaquedb-1.0.1/macaquedb.egg-info/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      268 2023-07-31 17:08:00.000000 macaquedb-1.0.1/macaquedb.egg-info/PKG-INFO
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      377 2023-07-31 17:08:00.000000 macaquedb-1.0.1/macaquedb.egg-info/SOURCES.txt
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        1 2023-07-31 17:08:00.000000 macaquedb-1.0.1/macaquedb.egg-info/dependency_links.txt
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       14 2023-07-31 17:08:00.000000 macaquedb-1.0.1/macaquedb.egg-info/requires.txt
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       10 2023-07-31 17:08:00.000000 macaquedb-1.0.1/macaquedb.egg-info/top_level.txt
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       38 2023-07-31 17:08:00.438506 macaquedb-1.0.1/setup.cfg
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      372 2023-07-31 17:07:05.000000 macaquedb-1.0.1/setup.py
```

### Comparing `macaquedb-1.0.0/macaquedb/Database.py` & `macaquedb-1.0.1/macaquedb/Database.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,91 @@
 # This file will be for connecting to the database, building, pulling data, etc.
 
 import os
 import sqlite3
 import re
 import csv
 import pandas as pd
-from .database.Subject import Subject
-from .database.Session import Session
-from .database.Image import Image
-from .database.utilities import *
+from database.Subject import Subject
+from database.Session import Session
+from database.Image import Image
+from database.utilities import *
 
 
 class Database:
 
     def __init__(self, db_path):
         self.db_path = db_path
         self.connect()
 
     def connect(self):
         self.conn = sqlite3.connect(self.db_path)
         self.cursor = self.conn.cursor()
 
     '''
-    Inserting data through a directory (populating subject tables, session tables, image tables, JSON tables)
-    '''
-
-    def input(self, data_dir):
-        # Inputting data into the table into table
-        self.insert_data(data_dir)
-        return
-
-    '''
     Loop through all subjects in a 'site-' dir and populate or update into the database
     '''
 
-    def insert_data(self, data_dir):
+    def input_site(self, data_dir, force=False):
         site_name = os.path.basename(data_dir)
         for subject in os.listdir(data_dir):
             subject_dir = os.path.join(data_dir, subject)
             # Check if the item is a directory
             if os.path.isdir(subject_dir) and subject.startswith("sub-"):
                 subject_id = subject[len('sub-'):]
                 session_count = self.loop_sessions(
-                    subject_dir=subject_dir, site_name=site_name, subject_id=subject_id)
+                    subject_dir=subject_dir, site_name=site_name, subject_id=subject_id, force=force)
                 new_sub = Subject(subject_id=subject_id,
                                   site=site_name,
                                   sessions=session_count)
-                self.insert_subject(new_sub)
+                self.insert_subject(new_sub, force)
+
+    '''
+    Input one specific subject
+    '''
+
+    def input_subject(self, subject_dir, site_name, force=False):
+        subject_id = os.path.basename(subject_dir)
+        subject_id = subject_id[len('sub-'):]
+        session_count = self.loop_session(
+            subject_dir=subject_dir, site_name=site_name, subject_id=subject_id, force=force)
+        new_sub = Subject(subject_id=subject_id,
+                          site=site_name,
+                          sessions=session_count)
+        self.insert_subject(new_sub, force)
 
     '''
     Loop over subjects in dir
     Returns session count for one subject
     '''
 
-    def loop_sessions(self, subject_dir, site_name, subject_id):
+    def loop_sessions(self, subject_dir, site_name, subject_id, force=False):
         session_count = 0
         for session in os.listdir(subject_dir):
             session_path = os.path.join(subject_dir, session)
             if os.path.isdir(session_path) and session.startswith('ses-'):
-                unique_id = subject_id + '_' + session
+                unique_id = subject_id + '_' + session[len('ses-'):]
                 # Also loop all the images within this session
                 image_count = self.loop_images(
-                    session_dir=session_path, subject_id=subject_id, session_id=unique_id, site=site_name)
+                    session_dir=session_path, subject_id=subject_id, session_id=unique_id, site=site_name, force=force)
                 new_session = Session(session_id=unique_id,
                                       subject_id=subject_id,
                                       site=site_name,
                                       image_count=image_count)
-                self.insert_session(new_session)
+                self.insert_session(new_session, force)
 
                 session_count += 1
 
         return session_count
 
     '''
     Loop over NIFTI files in a directory and add them all to the database
     '''
 
-    def loop_images(self, session_dir, subject_id, session_id, site):
+    def loop_images(self, session_dir, subject_id, session_id, site, force=False):
         # Walk through every file in session (anat, dwi, fieldmap, func)
         image_count = 1
         for root, dirs, files in os.walk(session_dir):
             for file in files:
                 file_path = os.path.join(root, file)
                 abs_file_path = os.path.abspath(file)
                 # Get file type and subtype
@@ -94,36 +99,43 @@
                     else:
                         image_subtype = "unknown"
                 elif image_type == "func":
                     if re.search(r"bold", file) or re.search(r"BOLD", file):
                         image_subtype = "bold"
                     else:
                         image_subtype = "unknown"
+                elif image_type == "dwi":
+                    if re.search(r"AP", file) or re.search(r"ap", file):
+                        image_subtype = "AP"
+                    elif re.search(r"PA", file) or re.search(r"pa", file):
+                        image_subtype = "PA"
+                    else:
+                        image_subtype = "unknown"
                 if is_nifti_file(file_path):
                     new_image = Image(image_id=file,
                                       session_id=session_id,
                                       subject_id=subject_id,
                                       image_type=os.path.basename(root),
                                       image_subtype=image_subtype,
                                       image_path=abs_file_path,
                                       run_number=image_count,
                                       site=site)
-                    self.insert_image(new_image)
+                    self.insert_image(new_image, force)
                     image_count += 1
 
         return image_count
 
     '''
     Function to add an image to the database
     '''
 
-    def insert_image(self, image):
+    def insert_image(self, image, force=False):
 
         # Check if it is in there already
-        query_check = "SELECT * FROM Image WHERE image_id = ?"
+        query_check = "SELECT * FROM Images WHERE image_id = ?"
         self.cursor.execute(query_check, (image.image_id,))
         existing_image = self.cursor.fetchone()
 
         attr_names = tuple(image.__dict__.keys())
 
         if existing_image:
             print("Image already exists in the database:")
@@ -136,39 +148,43 @@
             all_same = all(existing_image[i] == getattr(
                 image, attr) for i, attr in enumerate(attr_names))
 
             if all_same:
                 print("Image is already in database with same attributes, skipping")
                 return
 
-            choice = input("Do you want to update the existing image? (y/n)")
+            if force == False:
+                choice = input(
+                    "Do you want to update the existing image? (y/n)")
+            elif force == True:
+                choice = "y"
 
             if choice.lower() == "y":
-                query_update = f"UPDATE Image SET {', '.join(f'{name} = ?' for name in attr_names)} WHERE image_id = ?"
+                query_update = f"UPDATE Images SET {', '.join(f'{name} = ?' for name in attr_names)} WHERE image_id = ?"
                 values = new_row_values + (image.image_id,)
                 self.cursor.execute(query_update, values)
                 self.conn.commit()
                 print("Image updated successfully.")
             else:
                 print("Image not updated.")
         else:
-            query_insert = f"INSERT INTO Image {attr_names} VALUES ({', '.join(['?' for _ in attr_names])})"
+            query_insert = f"INSERT INTO Images {attr_names} VALUES ({', '.join(['?' for _ in attr_names])})"
             values = tuple(getattr(image, attr) for attr in attr_names)
             self.cursor.execute(query_insert, values)
             self.conn.commit()
             print(f"Image {image.image_id} inserted successfully.")
 
     '''
     Adding a specific session to the database
     '''
 
-    def insert_session(self, session):
+    def insert_session(self, session, force=False):
 
         # Check if it is in there already
-        query_check = "SELECT * FROM Session WHERE session_id = ?"
+        query_check = "SELECT * FROM Sessions WHERE session_id = ?"
         self.cursor.execute(query_check, (session.session_id,))
         existing_session = self.cursor.fetchone()
 
         attr_names = tuple(session.__dict__.keys())
 
         if existing_session:
             print("Session already exists in the database:")
@@ -182,37 +198,41 @@
             all_same = all(existing_session[i] == getattr(
                 session, attr) for i, attr in enumerate(attr_names))
 
             if all_same:
                 print("Session has no columns to update, skipping")
                 return
 
-            choice = input("Do you want to update the existing session? (y/n)")
+            if force == False:
+                choice = input(
+                    "Do you want to update the existing session? (y/n)")
+            elif force == True:
+                choice = "y"
 
             if choice.lower() == "y":
-                query_update = f"UPDATE Session SET {', '.join(f'{name} = ?' for name in attr_names)} WHERE session_id = ?"
+                query_update = f"UPDATE Sessions SET {', '.join(f'{name} = ?' for name in attr_names)} WHERE session_id = ?"
                 values = new_row_values + (session.session_id,)
                 self.cursor.execute(query_update, values)
                 self.conn.commit()
                 print("Session updated successfully.")
             else:
                 print("Session not updated.")
         else:
-            query_insert = f"INSERT INTO Session {attr_names} VALUES ({', '.join(['?' for _ in attr_names])})"
+            query_insert = f"INSERT INTO Sessions {attr_names} VALUES ({', '.join(['?' for _ in attr_names])})"
             values = tuple(getattr(session, attr) for attr in attr_names)
             self.cursor.execute(query_insert, values)
             self.conn.commit()
             print(f"Session {session.session_id} inserted successfully.")
 
     '''
     Takes in a subject class and inserts it into the database (checking whether it needs to be updated first)
     '''
 
-    def insert_subject(self, subject):
-        query_check = "SELECT * FROM Subject WHERE subject_id = ?"
+    def insert_subject(self, subject, force=False):
+        query_check = "SELECT * FROM Subjects WHERE subject_id = ?"
         self.cursor.execute(query_check, (subject.subject_id,))
         existing_subject = self.cursor.fetchone()
 
         attr_names = tuple(subject.__dict__.keys())
 
         if existing_subject:
             print("Subject already exists in the database:")
@@ -226,82 +246,171 @@
             all_same = all(existing_subject[i] == getattr(
                 subject, attr) for i, attr in enumerate(attr_names))
 
             if all_same:
                 print("Subject has no columns to update, skipping")
                 return
 
-            choice = input(
-                "Do you want to update the existing subject? (y/n): ")
+            if force == False:
+                choice = input(
+                    "Do you want to update the existing subject? (y/n): ")
+            elif force == True:
+                choice = "y"
 
             if choice.lower() == 'y':
-                query_update = f"UPDATE Subject SET {', '.join(f'{name} = ?' for name in attr_names)} WHERE subject_id = ?"
+                query_update = f"UPDATE Subjects SET {', '.join(f'{name} = ?' for name in attr_names)} WHERE subject_id = ?"
                 values = new_row_values + (subject.subject_id,)
                 self.cursor.execute(query_update, values)
                 self.conn.commit()
                 print("Subject updated successfully.")
             else:
                 print("Subject not updated.")
         else:
-            query_insert = f"INSERT INTO Subject {attr_names} VALUES ({', '.join(['?' for _ in attr_names])})"
+            query_insert = f"INSERT INTO Subjects {attr_names} VALUES ({', '.join(['?' for _ in attr_names])})"
             values = tuple(getattr(subject, attr) for attr in attr_names)
             self.cursor.execute(query_insert, values)
             self.conn.commit()
             print(f"Subject {subject.subject_id} inserted successfully.")
 
     def to_csv(self, csv_path, table_name, index=False):
         table = pd.read_sql(f"SELECT * FROM {table_name}", self.conn)
         table.to_csv(csv_path, index=index)
 
+    '''
+    Function to insert demographic information into the database
+    '''
+
+    def insert_demographics(self, csv_path, subject_column, session_column, age_column, sex_column):
+        df = pd.read_csv(csv_path, dtype={
+                         subject_column: str, session_column: str, age_column: str})
+        for index, row in df.iterrows():
+            csv_subject_id = row[subject_column]
+            csv_session_id = row[session_column]
+            csv_age = row[age_column]
+            csv_sex = row[sex_column]
+
+            sql_session_id = f"{csv_subject_id}_{csv_session_id}"
+
+            sex_query = f"""
+                INSERT INTO Subjects (subject_id, sex)
+                Values (?, ?)
+                ON CONFLICT(subject_id) DO UPDATE SET sex = excluded.sex
+             """
+
+            self.cursor.execute(sex_query, (csv_subject_id, csv_sex))
+            self.conn.commit()
+
+            age_query = f"""
+                INSERT INTO Sessions (session_id, age)
+                Values (?, ?)
+                ON CONFLICT(session_id) DO UPDATE SET age = excluded.age
+             """
+
+            self.cursor.execute(age_query, (sql_session_id, csv_age))
+            self.conn.commit()
+
+        return
+
+    '''
+    Function that prints all the colnames from each table
+    '''
+
+    def getColumnNames(self):
+        self.cursor.execute(
+            "SELECT name FROM sqlite_master WHERE type='table';")
+        tables = self.cursor.fetchall()
+        unique_columns = set()
+        for table in tables:
+            table_name = table[0]
+            self.cursor.execute(f"PRAGMA table_info({table_name});")
+            columns = self.cursor.fetchall()
+            column_names = [column[1] for column in columns]
+            unique_columns.update(column_names)
+        return unique_columns
+
+    '''
+    Function to take in column names and return a CSV file with those colnames
+    Also returns a pandas dataframe if you want it :)
+    '''
+
+    def make_csv(self, col_names, output_file):
+        all_columns = set()
+        for table_name in self.cursor.execute("SELECT name FROM sqlite_master WHERE type='table';").fetchall():
+            columns = self.cursor.execute(
+                f"PRAGMA table_info({table_name[0]});").fetchall()
+            all_columns.update(column[1] for column in columns)
+        invalid_columns = set(col_names) - all_columns
+        if invalid_columns:
+            print(f"Invalid column names: {', '.join(invalid_columns)}")
+            return
+
+        # Perform JOIN on relevant tables based on subject_id
+        query = """
+            SELECT * FROM Subjects
+            JOIN Sessions ON Subjects.subject_id = Sessions.subject_id
+            JOIN Images ON Subjects.subject_id = Images.subject_id;
+        """
+
+        # Fetch data from the JOINed tables using pandas
+        self.cursor.execute(query)
+        data = self.cursor.fetchall()
+        column_names = [col[0] for col in self.cursor.description]
+        df = pd.DataFrame(data, columns=column_names)
+        df = df[col_names]
+        df = df.loc[:, ~df.columns.duplicated()]
+        df.to_csv(output_file, index=False)
+
+        return (df)
+
     def to_table(self, table_name):
         table = pd.read_sql(f"SELECT * FROM {table_name}", self.conn)
         return table
 
     def build(self):
         self.cursor.execute('''
-            CREATE TABLE IF NOT EXISTS Subject (
+            CREATE TABLE IF NOT EXISTS Subjects (
                 subject_id TEXT PRIMARY KEY,
                 site TEXT,
                 sessions INTEGER,
-                gender TEXT CHECK(gender IN ('MALE', 'FEMALE'))
+                sex TEXT CHECK(sex IN ('M', 'F'))
             )
         ''')
 
         self.cursor.execute('''
-            CREATE TABLE IF NOT EXISTS Session (
+            CREATE TABLE IF NOT EXISTS Sessions (
                 session_id TEXT PRIMARY KEY,
                 subject_id TEXT,
                 age DOUBLE,
                 site TEXT,
                 image_count INT,
-                FOREIGN KEY (subject_id) REFERENCES Subject (subject_id)
+                FOREIGN KEY (subject_id) REFERENCES Subjects (subject_id)
             )
         ''')
 
         self.cursor.execute('''
-            CREATE TABLE IF NOT EXISTS Image (
+            CREATE TABLE IF NOT EXISTS Images (
                 image_id TEXT PRIMARY KEY,
                 session_id TEXT,
                 subject_id TEXT,
                 image_type TEXT,
                 image_subtype TEXT,
                 image_path TEXT,
                 mask_path TEXT,
                 run_number INTEGER,
                 site TEXT,
-                FOREIGN KEY (session_id) REFERENCES Session (session_id)
+                FOREIGN KEY (session_id) REFERENCES Sessions (session_id)
             )
         ''')
 
         self.cursor.execute('''
-            CREATE TABLE IF NOT EXISTS JSON (
+            CREATE TABLE IF NOT EXISTS JSONS (
                 json_id INTEGER PRIMARY KEY,
                 image_id INTEGER,
                 json_path TEXT,
-                FOREIGN KEY (image_id) REFERENCES Image (image_id)
+                FOREIGN KEY (image_id) REFERENCES Images (image_id)
             )
         ''')
 
         self.conn.commit()
         return
 
     def changePath(self, db_path):
@@ -326,7 +435,11 @@
         except sqlite3.Error as e:
             print(e)
 
         return
 
     def close(self):
         self.conn.close()
+
+    def getPath(self):
+        print(f"Current db path: {self.db_path}")
+        return
```

