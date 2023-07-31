# Comparing `tmp/iluxaMod-2.8.tar.gz` & `tmp/iluxaMod-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iluxaMod-2.8.tar", last modified: Mon Jul 31 16:33:33 2023, max compression
+gzip compressed data, was "iluxaMod-2.9.tar", last modified: Mon Jul 31 16:40:18 2023, max compression
```

## Comparing `iluxaMod-2.8.tar` & `iluxaMod-2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 16:33:33.590611 iluxaMod-2.8/
--rw-rw-rw-   0        0        0     5387 2023-07-31 16:33:33.589591 iluxaMod-2.8/PKG-INFO
--rw-rw-rw-   0        0        0     4466 2023-07-31 16:25:53.000000 iluxaMod-2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 16:33:33.581474 iluxaMod-2.8/iluxaMod/
--rw-rw-rw-   0        0        0       24 2023-07-31 16:09:15.000000 iluxaMod-2.8/iluxaMod/__init__.py
--rw-rw-rw-   0        0        0    21458 2023-07-31 16:25:53.000000 iluxaMod-2.8/iluxaMod/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:33:33.588590 iluxaMod-2.8/iluxaMod.egg-info/
--rw-rw-rw-   0        0        0     5387 2023-07-31 16:33:33.000000 iluxaMod-2.8/iluxaMod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-07-31 16:33:33.000000 iluxaMod-2.8/iluxaMod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 16:33:33.000000 iluxaMod-2.8/iluxaMod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-07-31 16:33:33.000000 iluxaMod-2.8/iluxaMod.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 16:33:33.000000 iluxaMod-2.8/iluxaMod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 16:33:33.590611 iluxaMod-2.8/setup.cfg
--rw-rw-rw-   0        0        0     1765 2023-07-31 16:33:29.000000 iluxaMod-2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:40:18.492889 iluxaMod-2.9/
+-rw-rw-rw-   0        0        0     5516 2023-07-31 16:40:18.491886 iluxaMod-2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4595 2023-07-31 16:36:57.000000 iluxaMod-2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 16:40:18.483848 iluxaMod-2.9/iluxaMod/
+-rw-rw-rw-   0        0        0       24 2023-07-31 16:09:15.000000 iluxaMod-2.9/iluxaMod/__init__.py
+-rw-rw-rw-   0        0        0    21458 2023-07-31 16:25:53.000000 iluxaMod-2.9/iluxaMod/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:40:18.490377 iluxaMod-2.9/iluxaMod.egg-info/
+-rw-rw-rw-   0        0        0     5516 2023-07-31 16:40:18.000000 iluxaMod-2.9/iluxaMod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-31 16:40:18.000000 iluxaMod-2.9/iluxaMod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 16:40:18.000000 iluxaMod-2.9/iluxaMod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-07-31 16:40:18.000000 iluxaMod-2.9/iluxaMod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 16:40:18.000000 iluxaMod-2.9/iluxaMod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 16:40:18.492889 iluxaMod-2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1765 2023-07-31 16:40:14.000000 iluxaMod-2.9/setup.py
```

### Comparing `iluxaMod-2.8/PKG-INFO` & `iluxaMod-2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iluxaMod
-Version: 2.8
+Version: 2.9
 Summary: Module for simplified work with libraries: TG, PostgreSQL, locations and more...
 Home-page: https://sbdt.pro
 Author: Illya Lazarev
 Author-email: lazarevillya031@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
@@ -39,20 +39,20 @@
 
 # Python PostgreSQL Module
  This python module is designed to interact with PostgreSQL databases. It provides an interface to create, read, update and delete records in various tables. The module is designed with a class  `postgreSQL`  that has various methods to interact with the database.
  ## Installation
  This module requires  `psycopg2`  package. Install it using pip:
 
 ```
-pip install psycopg2
+pip install iluxaMod
 ```
 ## Usage
  First, import the module:
 ```
-from postgreSQL import postgreSQL
+from iluxaMod import postgreSQL
 ```
 Then, create an instance of the  `postgreSQL`  class:
 ```
 db = postgreSQL(user="username", password="password", database="database_name", host="localhost")
 ```
 ### Methods
  Here are the methods provided by the  `postgreSQL`  class:
@@ -90,34 +90,42 @@
 Dropping the 'balance' table:
 ```
 db.drop_table(table="balance")
 ```
 # Convertors Class
  The Convertors class provides methods for converting between different image formats.
 ```
+from iluxaMod import Convertors
+
 convertor = Convertors('input.webp')
 convertor.webp2png('output.png')  # Convert a .webp file to .png
 convertor.webp2jpeg('output.jpeg')  # Convert a .webp file to .jpeg
 convertor.png2jpeg('output.jpeg')  # Convert a .png file to .jpeg
 convertor.jpeg2png('output.png')  # Convert a .jpeg file to .png
 convertor.png2ico('output.ico')  # Convert a .png file to .ico
 convertor.jpeg2ico('output.ico')  # Convert a .jpeg file to .ico
 ```
 ## Automation Ce Automation class provides methods for automating tasks.
 ```
+from iluxaMod import Automation
+
 no_ip = Automation.NoIp()
 no_ip.update('username', 'password')  # Update No-IP
 request = Automation.Requests()
 response = request.post('http://example.com', {'key': 'value'})  # Send a POST request
 ```
 ## Termux Class
  The Termux class provides methods for executing commands in Termux.
 ```
+from iluxaMod import Termux
+
 output = Termux.execute('ls')  # Execute a command
 battery_percentage = Termux.buttery_check()  # Check the battery status
 ```
 ## Tools Class
  The Tools class provides utility methods.
 ```
+from iluxaMod import Tools
+
 date = Tools.str2date('2022-01-01 00:00:00.000000')  # Convert a string to a datetime object
 Please note that all these classes and methods are provided as-is and may need to be adapted to suit your specific needs.
 ```
```

### Comparing `iluxaMod-2.8/README.md` & `iluxaMod-2.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 
 # Python PostgreSQL Module
  This python module is designed to interact with PostgreSQL databases. It provides an interface to create, read, update and delete records in various tables. The module is designed with a class  `postgreSQL`  that has various methods to interact with the database.
  ## Installation
  This module requires  `psycopg2`  package. Install it using pip:
 
 ```
-pip install psycopg2
+pip install iluxaMod
 ```
 ## Usage
  First, import the module:
 ```
-from postgreSQL import postgreSQL
+from iluxaMod import postgreSQL
 ```
 Then, create an instance of the  `postgreSQL`  class:
 ```
 db = postgreSQL(user="username", password="password", database="database_name", host="localhost")
 ```
 ### Methods
  Here are the methods provided by the  `postgreSQL`  class:
@@ -69,34 +69,42 @@
 Dropping the 'balance' table:
 ```
 db.drop_table(table="balance")
 ```
 # Convertors Class
  The Convertors class provides methods for converting between different image formats.
 ```
+from iluxaMod import Convertors
+
 convertor = Convertors('input.webp')
 convertor.webp2png('output.png')  # Convert a .webp file to .png
 convertor.webp2jpeg('output.jpeg')  # Convert a .webp file to .jpeg
 convertor.png2jpeg('output.jpeg')  # Convert a .png file to .jpeg
 convertor.jpeg2png('output.png')  # Convert a .jpeg file to .png
 convertor.png2ico('output.ico')  # Convert a .png file to .ico
 convertor.jpeg2ico('output.ico')  # Convert a .jpeg file to .ico
 ```
 ## Automation Ce Automation class provides methods for automating tasks.
 ```
+from iluxaMod import Automation
+
 no_ip = Automation.NoIp()
 no_ip.update('username', 'password')  # Update No-IP
 request = Automation.Requests()
 response = request.post('http://example.com', {'key': 'value'})  # Send a POST request
 ```
 ## Termux Class
  The Termux class provides methods for executing commands in Termux.
 ```
+from iluxaMod import Termux
+
 output = Termux.execute('ls')  # Execute a command
 battery_percentage = Termux.buttery_check()  # Check the battery status
 ```
 ## Tools Class
  The Tools class provides utility methods.
 ```
+from iluxaMod import Tools
+
 date = Tools.str2date('2022-01-01 00:00:00.000000')  # Convert a string to a datetime object
 Please note that all these classes and methods are provided as-is and may need to be adapted to suit your specific needs.
 ```
```

### Comparing `iluxaMod-2.8/iluxaMod/tools.py` & `iluxaMod-2.9/iluxaMod/tools.py`

 * *Files identical despite different names*

### Comparing `iluxaMod-2.8/iluxaMod.egg-info/PKG-INFO` & `iluxaMod-2.9/iluxaMod.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iluxaMod
-Version: 2.8
+Version: 2.9
 Summary: Module for simplified work with libraries: TG, PostgreSQL, locations and more...
 Home-page: https://sbdt.pro
 Author: Illya Lazarev
 Author-email: lazarevillya031@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
@@ -39,20 +39,20 @@
 
 # Python PostgreSQL Module
  This python module is designed to interact with PostgreSQL databases. It provides an interface to create, read, update and delete records in various tables. The module is designed with a class  `postgreSQL`  that has various methods to interact with the database.
  ## Installation
  This module requires  `psycopg2`  package. Install it using pip:
 
 ```
-pip install psycopg2
+pip install iluxaMod
 ```
 ## Usage
  First, import the module:
 ```
-from postgreSQL import postgreSQL
+from iluxaMod import postgreSQL
 ```
 Then, create an instance of the  `postgreSQL`  class:
 ```
 db = postgreSQL(user="username", password="password", database="database_name", host="localhost")
 ```
 ### Methods
  Here are the methods provided by the  `postgreSQL`  class:
@@ -90,34 +90,42 @@
 Dropping the 'balance' table:
 ```
 db.drop_table(table="balance")
 ```
 # Convertors Class
  The Convertors class provides methods for converting between different image formats.
 ```
+from iluxaMod import Convertors
+
 convertor = Convertors('input.webp')
 convertor.webp2png('output.png')  # Convert a .webp file to .png
 convertor.webp2jpeg('output.jpeg')  # Convert a .webp file to .jpeg
 convertor.png2jpeg('output.jpeg')  # Convert a .png file to .jpeg
 convertor.jpeg2png('output.png')  # Convert a .jpeg file to .png
 convertor.png2ico('output.ico')  # Convert a .png file to .ico
 convertor.jpeg2ico('output.ico')  # Convert a .jpeg file to .ico
 ```
 ## Automation Ce Automation class provides methods for automating tasks.
 ```
+from iluxaMod import Automation
+
 no_ip = Automation.NoIp()
 no_ip.update('username', 'password')  # Update No-IP
 request = Automation.Requests()
 response = request.post('http://example.com', {'key': 'value'})  # Send a POST request
 ```
 ## Termux Class
  The Termux class provides methods for executing commands in Termux.
 ```
+from iluxaMod import Termux
+
 output = Termux.execute('ls')  # Execute a command
 battery_percentage = Termux.buttery_check()  # Check the battery status
 ```
 ## Tools Class
  The Tools class provides utility methods.
 ```
+from iluxaMod import Tools
+
 date = Tools.str2date('2022-01-01 00:00:00.000000')  # Convert a string to a datetime object
 Please note that all these classes and methods are provided as-is and may need to be adapted to suit your specific needs.
 ```
```

### Comparing `iluxaMod-2.8/setup.py` & `iluxaMod-2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = str(f.read())
 
 setup(
     name='iluxaMod',
-    version='2.8',  # Версия вашего пакета
+    version='2.9',  # Версия вашего пакета
     packages=['iluxaMod'],  # Автоматически найдет все пакеты в корневой директории
     install_requires=[  # Зависимости вашего пакета
         'geopy',
         'psycopg2-binary',
         'pyTelegramBotAPI',
         'requests',
         'pyfirmata',
```

