# Comparing `tmp/hotel_manage_soumya-0.0.5.tar.gz` & `tmp/hotel_manage_soumya-0.0.6.tar.gz`

## Comparing `hotel_manage_soumya-0.0.5.tar` & `hotel_manage_soumya-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    15697 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.5/result.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.5/src/hotel_manage_soumya/__init__.py
--rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.5/src/hotel_manage_soumya/booking.py
--rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.5/src/hotel_manage_soumya/room.py
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.5/src/hotel_manage_soumya/user.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.5/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.5/LICENSE
--rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.5/README.md
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    15697 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.6/result.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.6/src/hotel_manage_soumya/__init__.py
+-rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.6/src/hotel_manage_soumya/booking.py
+-rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.6/src/hotel_manage_soumya/room.py
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.6/src/hotel_manage_soumya/user.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.6/README.md
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 hotel_manage_soumya-0.0.6/PKG-INFO
```

### Comparing `hotel_manage_soumya-0.0.5/result.png` & `hotel_manage_soumya-0.0.6/result.png`

 * *Files identical despite different names*

### Comparing `hotel_manage_soumya-0.0.5/src/hotel_manage_soumya/booking.py` & `hotel_manage_soumya-0.0.6/src/hotel_manage_soumya/booking.py`

 * *Files identical despite different names*

### Comparing `hotel_manage_soumya-0.0.5/src/hotel_manage_soumya/room.py` & `hotel_manage_soumya-0.0.6/src/hotel_manage_soumya/room.py`

 * *Files identical despite different names*

### Comparing `hotel_manage_soumya-0.0.5/src/hotel_manage_soumya/user.py` & `hotel_manage_soumya-0.0.6/src/hotel_manage_soumya/user.py`

 * *Files identical despite different names*

### Comparing `hotel_manage_soumya-0.0.5/LICENSE` & `hotel_manage_soumya-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hotel_manage_soumya-0.0.5/README.md` & `hotel_manage_soumya-0.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,96 +21,111 @@
 
 ## Prerequisite
 * Python >=3.7
 * AWS Account
 * DynamoDB connection
 * Flask
 
+## How to use library in Flask APP
+Following Flask app will return the total number of bookings, total number of rooms and total number of users. Follow steps to start Flask APP.
+### Step 1: Create virtual environment
+```python
+# Create directory
+mkdir hotel_management
+
+# Change directory
+cd hotel_management
 
-## Installation
-Install library using following command
-```bash
-  pip install hotel-manage-soumya
-```
-
-## Usage/Examples
-Following Flask app will return the total number of bookings, total number of rooms and total number of users.
+# Create and activate virtual environment
+python -m venv .venv
 
-**`Note:`** Make sure you already have tables with data in DynamoDB and if you still face any issue then you can contact with us or explore the Class, Function from Github [Hotel-manage-soumya](https://github.com/soumyak96/hotel_manage_soumya) and directory `src/hotel_manage_soumya`.
+# For Window:
+source .venv/Scripts/activate
 
-```javascript
+# For Ubuntu:
+source .venv/bin/activate
+```
+### Step 2: Create Flask APP
+Copy following code and save into app.py
+```python
 from flask import Flask
-from dotenv import load_dotenv
 import boto3
-import os
 
-
-// Import classes from hotel_manage_soumya
+# Import classes from hotel_manage_soumya
 from hotel_manage_soumya.booking import Booking
 from hotel_manage_soumya.room import Room
 from hotel_manage_soumya.user import User
 
 load_dotenv()
 app = Flask(__name__)
 app.secret_key = 'your_secret_key'
 
-// Initialize the DynamoDB client
+# Initialize the DynamoDB client
 dynamodb =  boto3.client(
                 'dynamodb', 
-                aws_access_key_id=os.environ['AWS_ACCESS_KEY_ID'],
-                aws_secret_access_key=os.environ['AWS_SECRET_ACCESS_KEY'],
-                region_name=os.environ['AWS_REGION']
+                aws_access_key_id='YOUR_AWS_ACCESS_KEY_ID',
+                aws_secret_access_key='YOUR_AWS_SECRET_ACCESS_KEY',
+                region_name='us-east-1'
             )
 
-// Initialize classes objects
+# Initialize classes objects
 tableName = 'bookings'
 booking_obj = Booking(tableName)
 
 roomTableName = 'rooms'
 bucketName = 'hotel-management-soumya'
 room_obj = Room(roomTableName, bucketName)
 
 userTableName = 'users'
 user_obj = User(userTableName)
 
 @app.route('/', methods=['GET'])
 def home():
-    //  All Bookings
+    # All Bookings
     all_booking = booking_obj.get_all_booking(dynamodb)
     total_booking = len(all_booking['data']['Items'])
 
-    //  All Rooms
+    # All Rooms
     all_rooms = room_obj.get_all_room(dynamodb)
     total_room = len(all_rooms['data']['Items'])
 
-    //  All users
+    # All users
     all_users = user_obj.get_all_user(dynamodb)
     total_users = len(all_users['data']['Items'])
     
     return {
         "statusCode": 200,
         "TotalBooking": total_booking,
         "TotalRoom": total_room,
         "TotalUser": total_users
     }
 ```
-
+### Step 3: Install dependencies
+```python
+pip install hotel-manage-soumya
+pip install flask
+pip install boto3
+```
 #### Flask APP Response
-```javascript
+```python
 {
   "TotalBooking": 4,
   "TotalRoom": 4,
   "TotalUser": 3,
   "statusCode": 200
 }
 
 ```
+### Step 4: Start Server
+```python
+python app.py OR flask run
+```
 
+**`Note:`** Make sure you already have tables with data in DynamoDB and if you still face any issue then you can contact with us or explore the Class, Function from Github [Hotel-manage-soumya](https://github.com/soumyak96/hotel_manage_soumya) and directory `src/hotel_manage_soumya`.
 
-## Support
-
-For support, email x21174059@student.ncirl.ie , soumyaksoochik96@gmail.com.
 
 
+## Support
 
+For support, email x21174059@student.ncirl.ie , soumyaksoochik96@gmail.com.
```

### Comparing `hotel_manage_soumya-0.0.5/pyproject.toml` & `hotel_manage_soumya-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "hotel_manage_soumya"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
 { name="Soumya Ksoochik", email="soumyaksoochik96@gmail.com" },
 ]
 description = "Hotel-Manage-Soumya is a lightweight Python library designed to simplify and streamline the management of bookings, rooms, and users within Flask web applications. With its easy-to-use classes and methods, it provides a set of essential functionalities for handling booking management, room management, and user management."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `hotel_manage_soumya-0.0.5/PKG-INFO` & `hotel_manage_soumya-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotel_manage_soumya
-Version: 0.0.5
+Version: 0.0.6
 Summary: Hotel-Manage-Soumya is a lightweight Python library designed to simplify and streamline the management of bookings, rooms, and users within Flask web applications. With its easy-to-use classes and methods, it provides a set of essential functionalities for handling booking management, room management, and user management.
 Project-URL: Homepage, https://github.com/soumyak96/hotel_manage_soumya
 Project-URL: Bug Tracker, https://github.com/soumyak96/hotel_manage_soumya/issues
 Author-email: Soumya Ksoochik <soumyaksoochik96@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,96 +35,111 @@
 
 ## Prerequisite
 * Python >=3.7
 * AWS Account
 * DynamoDB connection
 * Flask
 
+## How to use library in Flask APP
+Following Flask app will return the total number of bookings, total number of rooms and total number of users. Follow steps to start Flask APP.
+### Step 1: Create virtual environment
+```python
+# Create directory
+mkdir hotel_management
+
+# Change directory
+cd hotel_management
 
-## Installation
-Install library using following command
-```bash
-  pip install hotel-manage-soumya
-```
-
-## Usage/Examples
-Following Flask app will return the total number of bookings, total number of rooms and total number of users.
+# Create and activate virtual environment
+python -m venv .venv
 
-**`Note:`** Make sure you already have tables with data in DynamoDB and if you still face any issue then you can contact with us or explore the Class, Function from Github [Hotel-manage-soumya](https://github.com/soumyak96/hotel_manage_soumya) and directory `src/hotel_manage_soumya`.
+# For Window:
+source .venv/Scripts/activate
 
-```javascript
+# For Ubuntu:
+source .venv/bin/activate
+```
+### Step 2: Create Flask APP
+Copy following code and save into app.py
+```python
 from flask import Flask
-from dotenv import load_dotenv
 import boto3
-import os
 
-
-// Import classes from hotel_manage_soumya
+# Import classes from hotel_manage_soumya
 from hotel_manage_soumya.booking import Booking
 from hotel_manage_soumya.room import Room
 from hotel_manage_soumya.user import User
 
 load_dotenv()
 app = Flask(__name__)
 app.secret_key = 'your_secret_key'
 
-// Initialize the DynamoDB client
+# Initialize the DynamoDB client
 dynamodb =  boto3.client(
                 'dynamodb', 
-                aws_access_key_id=os.environ['AWS_ACCESS_KEY_ID'],
-                aws_secret_access_key=os.environ['AWS_SECRET_ACCESS_KEY'],
-                region_name=os.environ['AWS_REGION']
+                aws_access_key_id='YOUR_AWS_ACCESS_KEY_ID',
+                aws_secret_access_key='YOUR_AWS_SECRET_ACCESS_KEY',
+                region_name='us-east-1'
             )
 
-// Initialize classes objects
+# Initialize classes objects
 tableName = 'bookings'
 booking_obj = Booking(tableName)
 
 roomTableName = 'rooms'
 bucketName = 'hotel-management-soumya'
 room_obj = Room(roomTableName, bucketName)
 
 userTableName = 'users'
 user_obj = User(userTableName)
 
 @app.route('/', methods=['GET'])
 def home():
-    //  All Bookings
+    # All Bookings
     all_booking = booking_obj.get_all_booking(dynamodb)
     total_booking = len(all_booking['data']['Items'])
 
-    //  All Rooms
+    # All Rooms
     all_rooms = room_obj.get_all_room(dynamodb)
     total_room = len(all_rooms['data']['Items'])
 
-    //  All users
+    # All users
     all_users = user_obj.get_all_user(dynamodb)
     total_users = len(all_users['data']['Items'])
     
     return {
         "statusCode": 200,
         "TotalBooking": total_booking,
         "TotalRoom": total_room,
         "TotalUser": total_users
     }
 ```
-
+### Step 3: Install dependencies
+```python
+pip install hotel-manage-soumya
+pip install flask
+pip install boto3
+```
 #### Flask APP Response
-```javascript
+```python
 {
   "TotalBooking": 4,
   "TotalRoom": 4,
   "TotalUser": 3,
   "statusCode": 200
 }
 
 ```
+### Step 4: Start Server
+```python
+python app.py OR flask run
+```
 
+**`Note:`** Make sure you already have tables with data in DynamoDB and if you still face any issue then you can contact with us or explore the Class, Function from Github [Hotel-manage-soumya](https://github.com/soumyak96/hotel_manage_soumya) and directory `src/hotel_manage_soumya`.
 
-## Support
-
-For support, email x21174059@student.ncirl.ie , soumyaksoochik96@gmail.com.
 
 
+## Support
 
+For support, email x21174059@student.ncirl.ie , soumyaksoochik96@gmail.com.
```

