# Comparing `tmp/macaquedb-1.0.2.tar.gz` & `tmp/macaquedb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macaquedb-1.0.2.tar", last modified: Mon Jul 31 17:52:48 2023, max compression
+gzip compressed data, was "macaquedb-1.0.3.tar", last modified: Mon Jul 31 18:34:57 2023, max compression
```

## Comparing `macaquedb-1.0.2.tar` & `macaquedb-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 17:52:48.808452 macaquedb-1.0.2/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      223 2023-07-31 17:52:48.808280 macaquedb-1.0.2/PKG-INFO
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)     2335 2023-07-28 16:05:19.000000 macaquedb-1.0.2/README.md
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 17:52:48.805991 macaquedb-1.0.2/macaquedb/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)    16721 2023-07-31 17:51:37.000000 macaquedb-1.0.2/macaquedb/Database.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       31 2023-07-21 17:03:41.000000 macaquedb-1.0.2/macaquedb/__init__.py
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 17:52:48.807930 macaquedb-1.0.2/macaquedb/database/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      489 2023-07-21 14:36:48.000000 macaquedb-1.0.2/macaquedb/database/Image.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      306 2023-07-21 14:36:48.000000 macaquedb-1.0.2/macaquedb/database/Session.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      294 2023-07-31 15:08:30.000000 macaquedb-1.0.2/macaquedb/database/Subject.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 16:58:35.000000 macaquedb-1.0.2/macaquedb/database/__init__.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      451 2023-07-21 14:36:48.000000 macaquedb-1.0.2/macaquedb/database/utilities.py
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 17:52:48.806908 macaquedb-1.0.2/macaquedb.egg-info/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      223 2023-07-31 17:52:48.000000 macaquedb-1.0.2/macaquedb.egg-info/PKG-INFO
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      377 2023-07-31 17:52:48.000000 macaquedb-1.0.2/macaquedb.egg-info/SOURCES.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        1 2023-07-31 17:52:48.000000 macaquedb-1.0.2/macaquedb.egg-info/dependency_links.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       14 2023-07-31 17:52:48.000000 macaquedb-1.0.2/macaquedb.egg-info/requires.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       10 2023-07-31 17:52:48.000000 macaquedb-1.0.2/macaquedb.egg-info/top_level.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       38 2023-07-31 17:52:48.808511 macaquedb-1.0.2/setup.cfg
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      372 2023-07-31 17:52:41.000000 macaquedb-1.0.2/setup.py
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 18:34:57.855874 macaquedb-1.0.3/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      223 2023-07-31 18:34:57.855676 macaquedb-1.0.3/PKG-INFO
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)     2335 2023-07-28 16:05:19.000000 macaquedb-1.0.3/README.md
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 18:34:57.853145 macaquedb-1.0.3/macaquedb/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)    17542 2023-07-31 18:30:34.000000 macaquedb-1.0.3/macaquedb/Database.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       31 2023-07-21 17:03:41.000000 macaquedb-1.0.3/macaquedb/__init__.py
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 18:34:57.855291 macaquedb-1.0.3/macaquedb/database/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      489 2023-07-21 14:36:48.000000 macaquedb-1.0.3/macaquedb/database/Image.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      306 2023-07-21 14:36:48.000000 macaquedb-1.0.3/macaquedb/database/Session.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      294 2023-07-31 15:08:30.000000 macaquedb-1.0.3/macaquedb/database/Subject.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 16:58:35.000000 macaquedb-1.0.3/macaquedb/database/__init__.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      451 2023-07-21 14:36:48.000000 macaquedb-1.0.3/macaquedb/database/utilities.py
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 18:34:57.854098 macaquedb-1.0.3/macaquedb.egg-info/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      223 2023-07-31 18:34:57.000000 macaquedb-1.0.3/macaquedb.egg-info/PKG-INFO
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      377 2023-07-31 18:34:57.000000 macaquedb-1.0.3/macaquedb.egg-info/SOURCES.txt
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        1 2023-07-31 18:34:57.000000 macaquedb-1.0.3/macaquedb.egg-info/dependency_links.txt
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       14 2023-07-31 18:34:57.000000 macaquedb-1.0.3/macaquedb.egg-info/requires.txt
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       10 2023-07-31 18:34:57.000000 macaquedb-1.0.3/macaquedb.egg-info/top_level.txt
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       38 2023-07-31 18:34:57.855944 macaquedb-1.0.3/setup.cfg
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      372 2023-07-31 18:34:22.000000 macaquedb-1.0.3/setup.py
```

### Comparing `macaquedb-1.0.2/README.md` & `macaquedb-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `macaquedb-1.0.2/macaquedb/Database.py` & `macaquedb-1.0.3/macaquedb/Database.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
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
@@ -284,33 +284,48 @@
                          subject_column: str, session_column: str, age_column: str})
         for index, row in df.iterrows():
             csv_subject_id = row[subject_column]
             csv_session_id = row[session_column]
             csv_age = row[age_column]
             csv_sex = row[sex_column]
 
-            sql_session_id = f"{csv_subject_id}_{csv_session_id}"
-
-            sex_query = f"""
-                INSERT INTO Subjects (subject_id, sex)
-                Values (?, ?)
-                ON CONFLICT(subject_id) DO UPDATE SET sex = excluded.sex
-             """
+            if csv_subject_id == "032213":
+                print(csv_subject_id)
 
-            self.cursor.execute(sex_query, (csv_subject_id, csv_sex))
-            self.conn.commit()
+            sql_session_id = f"{csv_subject_id}_{csv_session_id}"
 
-            age_query = f"""
-                INSERT INTO Sessions (session_id, age)
-                Values (?, ?)
-                ON CONFLICT(session_id) DO UPDATE SET age = excluded.age
-             """
+            # Check if the subject exists in the Subjects table
+            subject_query = "SELECT COUNT(*) FROM Subjects WHERE subject_id = ?"
+            self.cursor.execute(subject_query, (csv_subject_id,))
+            subject_exists = self.cursor.fetchone()[0]
+
+            if subject_exists:
+                # Insert or update the sex in Subjects table
+                sex_query = """
+                    INSERT INTO Subjects (subject_id, sex)
+                    VALUES (?, ?)
+                    ON CONFLICT(subject_id) DO UPDATE SET sex = excluded.sex
+                """
+                self.cursor.execute(sex_query, (csv_subject_id, csv_sex))
+                self.conn.commit()
 
-            self.cursor.execute(age_query, (sql_session_id, csv_age))
-            self.conn.commit()
+            # Check if the session exists in the Sessions table
+            session_query = "SELECT COUNT(*) FROM Sessions WHERE session_id = ?"
+            self.cursor.execute(session_query, (sql_session_id,))
+            session_exists = self.cursor.fetchone()[0]
+
+            if session_exists:
+                # Insert or update the age in Sessions table
+                age_query = """
+                    INSERT INTO Sessions (session_id, age)
+                    VALUES (?, ?)
+                    ON CONFLICT(session_id) DO UPDATE SET age = excluded.age
+                """
+                self.cursor.execute(age_query, (sql_session_id, csv_age))
+                self.conn.commit()
 
         return
 
     '''
     Function that prints all the colnames from each table
     '''
 
@@ -367,15 +382,15 @@
 
     def build(self):
         self.cursor.execute('''
             CREATE TABLE IF NOT EXISTS Subjects (
                 subject_id TEXT PRIMARY KEY,
                 site TEXT,
                 sessions INTEGER,
-                sex TEXT CHECK(sex IN ('M', 'F'))
+                sex TEXT
             )
         ''')
 
         self.cursor.execute('''
             CREATE TABLE IF NOT EXISTS Sessions (
                 session_id TEXT PRIMARY KEY,
                 subject_id TEXT,
```

