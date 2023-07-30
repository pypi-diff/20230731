# Comparing `tmp/BloxPy-0.1.11.tar.gz` & `tmp/BloxPy-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BloxPy-0.1.11.tar", last modified: Fri Jul 28 21:58:16 2023, max compression
+gzip compressed data, was "BloxPy-0.1.12.tar", last modified: Sun Jul 30 22:39:43 2023, max compression
```

## Comparing `BloxPy-0.1.11.tar` & `BloxPy-0.1.12.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 21:58:16.323167 BloxPy-0.1.11/
-drwxrwxrwx   0        0        0        0 2023-07-28 21:58:16.315171 BloxPy-0.1.11/BloxPy/
--rw-rw-rw-   0        0        0        0 2023-07-28 21:18:45.000000 BloxPy-0.1.11/BloxPy/__init__.py
--rw-rw-rw-   0        0        0      343 2023-07-28 20:19:36.000000 BloxPy-0.1.11/BloxPy/users.py
-drwxrwxrwx   0        0        0        0 2023-07-28 21:58:16.321168 BloxPy-0.1.11/BloxPy.egg-info/
--rw-rw-rw-   0        0        0     2921 2023-07-28 21:58:16.000000 BloxPy-0.1.11/BloxPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-28 21:58:16.000000 BloxPy-0.1.11/BloxPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 21:58:16.000000 BloxPy-0.1.11/BloxPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-28 21:58:16.000000 BloxPy-0.1.11/BloxPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 21:58:16.000000 BloxPy-0.1.11/BloxPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2921 2023-07-28 21:58:16.323167 BloxPy-0.1.11/PKG-INFO
--rw-rw-rw-   0        0        0     2016 2023-07-28 20:35:14.000000 BloxPy-0.1.11/README.md
--rw-rw-rw-   0        0        0       42 2023-07-28 21:58:16.323167 BloxPy-0.1.11/setup.cfg
--rw-rw-rw-   0        0        0     1740 2023-07-28 21:58:04.000000 BloxPy-0.1.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 22:39:43.284397 BloxPy-0.1.12/
+drwxrwxrwx   0        0        0        0 2023-07-30 22:39:43.271405 BloxPy-0.1.12/BloxPy/
+-rw-rw-rw-   0        0        0     6526 2023-07-30 21:44:32.000000 BloxPy-0.1.12/BloxPy/Groups.py
+-rw-rw-rw-   0        0        0     8147 2023-07-30 22:08:39.000000 BloxPy-0.1.12/BloxPy/Search.py
+-rw-rw-rw-   0        0        0     3093 2023-07-30 20:52:11.000000 BloxPy-0.1.12/BloxPy/Users.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 21:18:45.000000 BloxPy-0.1.12/BloxPy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 22:39:43.280399 BloxPy-0.1.12/BloxPy.egg-info/
+-rw-rw-rw-   0        0        0     3752 2023-07-30 22:39:43.000000 BloxPy-0.1.12/BloxPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-30 22:39:43.000000 BloxPy-0.1.12/BloxPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 22:39:43.000000 BloxPy-0.1.12/BloxPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 22:39:43.000000 BloxPy-0.1.12/BloxPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-30 22:39:43.000000 BloxPy-0.1.12/BloxPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3752 2023-07-30 22:39:43.283397 BloxPy-0.1.12/PKG-INFO
+-rw-rw-rw-   0        0        0     2839 2023-07-30 22:39:17.000000 BloxPy-0.1.12/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 22:39:43.282400 BloxPy-0.1.12/_exceptions/
+-rw-rw-rw-   0        0        0     1774 2023-07-30 22:02:04.000000 BloxPy-0.1.12/_exceptions/RobloxExceptions.py
+-rw-rw-rw-   0        0        0      428 2023-07-30 22:03:36.000000 BloxPy-0.1.12/_exceptions/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-30 22:39:43.285397 BloxPy-0.1.12/setup.cfg
+-rw-rw-rw-   0        0        0     1752 2023-07-30 21:31:03.000000 BloxPy-0.1.12/setup.py
```

### Comparing `BloxPy-0.1.11/BloxPy.egg-info/PKG-INFO` & `BloxPy-0.1.12/BloxPy.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: BloxPy
-Version: 0.1.11
-Summary: BloxPy: Your All-in-One Python Library for Roblox Development
-Home-page: https://github.com/yourusername/bloxpy
+Version: 0.1.12
+Summary: BloxPy: Your All-in-One Python API wrapper for Roblox Development
+Home-page: https://github.com/Developer-X-0001/BloxPy
 Author: Developer X
 Author-email: developer.x.business@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,22 +14,22 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-# BloxPy: Your All-in-One Python Library for Roblox Development
+# BloxPy: Your All-in-One Python API Wrapper for Roblox Development
 
-![BloxPy Logo](https://example.com/BloxPy_logo.png)
+![BloxPy Logo](BloxPy.png)
 
-BloxPy is the ultimate Python library for Roblox developers, offering an all-in-one solution to interact with Roblox Public APIs effortlessly. Whether you want to retrieve player data, manage groups, or create dynamic game interactions, BloxPy empowers you to build amazing Roblox experiences with ease.
+BloxPy is the ultimate Python API wrapper for Roblox developers, offering an all-in-one solution to interact with Roblox Public APIs effortlessly. Whether you want to retrieve player data, manage groups, or create dynamic game interactions, BloxPy empowers you to build amazing Roblox experiences with ease.
 
 [![License](https://img.shields.io/github/license/Developer-X-0001/BloxPy)](https://github.com/Developer-X-0001/BloxPy/blob/main/LICENSE)
 [![PyPI Version](https://img.shields.io/pypi/v/BloxPy)](https://pypi.org/project/BloxPy/)
 [![Python Version](https://img.shields.io/pypi/pyversions/BloxPy)](https://pypi.org/project/BloxPy/)
 
 ## Features
 
@@ -44,26 +44,58 @@
 
 ```bash
 pip install BloxPy
 ```
 
 ## Usage
 
+- ### Users
 ```py
-import BloxPy
+from BloxPy import Users
 
 # Fetch player data
 player_id = 1234567890
-player_data = BloxPy.get_player_data(player_id)
-print(player_data)
+player_data = Users.get_user(player_id)
+print(player_data.name) # Username
+print(player_data.displayName) # Display Name
+```
+
+- ### Groups
+```py
+from BloxPy import Groups
+
+# Fetch group data
+group_id = 1234567890
+group_data = Groups.get_group(group_id)
+print(group_data.name) # Group Name
+print(group_data.memberCount) # Group Member Count
+```
+
+- ### Search
+```py
+from BloxPy import Search
 
-# Manage groups
-group_id = 9876543210
-group_members = BloxPy.get_group_members(group_id)
-print(group_members)
+# Fetch users by keyword
+user_keyword = 'Henry'
+user_search_results = Search.search_users(keyword)
+print(user_search_results.data) # List containing data
+
+for user in user_search_results.data:
+    print(user.name) # Username
+    print(user.id) # User ID
+
+# Fetch groups by keyword
+group_keyword = 'Roblox'
+group_search_results = Search.search_groups(keyword)
+print(group_search_results.data) # List containing data
+
+for group in group_search_results.data:
+    print(group.name) # Name
+    print(group.description) # Description
+    print(group.memberCount) # Member Count
 ```
 
 ## Documentation
 
 For detailed documentation and usage examples, check out the [BloxPy Documentation](https://Developer-X-0001.github.io/BloxPy-docs).
 
 ## Contributing
```

### Comparing `BloxPy-0.1.11/PKG-INFO` & `BloxPy-0.1.12/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: BloxPy
-Version: 0.1.11
-Summary: BloxPy: Your All-in-One Python Library for Roblox Development
-Home-page: https://github.com/yourusername/bloxpy
+Version: 0.1.12
+Summary: BloxPy: Your All-in-One Python API wrapper for Roblox Development
+Home-page: https://github.com/Developer-X-0001/BloxPy
 Author: Developer X
 Author-email: developer.x.business@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,22 +14,22 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-# BloxPy: Your All-in-One Python Library for Roblox Development
+# BloxPy: Your All-in-One Python API Wrapper for Roblox Development
 
-![BloxPy Logo](https://example.com/BloxPy_logo.png)
+![BloxPy Logo](BloxPy.png)
 
-BloxPy is the ultimate Python library for Roblox developers, offering an all-in-one solution to interact with Roblox Public APIs effortlessly. Whether you want to retrieve player data, manage groups, or create dynamic game interactions, BloxPy empowers you to build amazing Roblox experiences with ease.
+BloxPy is the ultimate Python API wrapper for Roblox developers, offering an all-in-one solution to interact with Roblox Public APIs effortlessly. Whether you want to retrieve player data, manage groups, or create dynamic game interactions, BloxPy empowers you to build amazing Roblox experiences with ease.
 
 [![License](https://img.shields.io/github/license/Developer-X-0001/BloxPy)](https://github.com/Developer-X-0001/BloxPy/blob/main/LICENSE)
 [![PyPI Version](https://img.shields.io/pypi/v/BloxPy)](https://pypi.org/project/BloxPy/)
 [![Python Version](https://img.shields.io/pypi/pyversions/BloxPy)](https://pypi.org/project/BloxPy/)
 
 ## Features
 
@@ -44,26 +44,58 @@
 
 ```bash
 pip install BloxPy
 ```
 
 ## Usage
 
+- ### Users
 ```py
-import BloxPy
+from BloxPy import Users
 
 # Fetch player data
 player_id = 1234567890
-player_data = BloxPy.get_player_data(player_id)
-print(player_data)
+player_data = Users.get_user(player_id)
+print(player_data.name) # Username
+print(player_data.displayName) # Display Name
+```
+
+- ### Groups
+```py
+from BloxPy import Groups
+
+# Fetch group data
+group_id = 1234567890
+group_data = Groups.get_group(group_id)
+print(group_data.name) # Group Name
+print(group_data.memberCount) # Group Member Count
+```
+
+- ### Search
+```py
+from BloxPy import Search
 
-# Manage groups
-group_id = 9876543210
-group_members = BloxPy.get_group_members(group_id)
-print(group_members)
+# Fetch users by keyword
+user_keyword = 'Henry'
+user_search_results = Search.search_users(keyword)
+print(user_search_results.data) # List containing data
+
+for user in user_search_results.data:
+    print(user.name) # Username
+    print(user.id) # User ID
+
+# Fetch groups by keyword
+group_keyword = 'Roblox'
+group_search_results = Search.search_groups(keyword)
+print(group_search_results.data) # List containing data
+
+for group in group_search_results.data:
+    print(group.name) # Name
+    print(group.description) # Description
+    print(group.memberCount) # Member Count
 ```
 
 ## Documentation
 
 For detailed documentation and usage examples, check out the [BloxPy Documentation](https://Developer-X-0001.github.io/BloxPy-docs).
 
 ## Contributing
```

### Comparing `BloxPy-0.1.11/README.md` & `BloxPy-0.1.12/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# BloxPy: Your All-in-One Python Library for Roblox Development
+# BloxPy: Your All-in-One Python API Wrapper for Roblox Development
 
-![BloxPy Logo](https://example.com/BloxPy_logo.png)
+![BloxPy Logo](BloxPy.png)
 
-BloxPy is the ultimate Python library for Roblox developers, offering an all-in-one solution to interact with Roblox Public APIs effortlessly. Whether you want to retrieve player data, manage groups, or create dynamic game interactions, BloxPy empowers you to build amazing Roblox experiences with ease.
+BloxPy is the ultimate Python API wrapper for Roblox developers, offering an all-in-one solution to interact with Roblox Public APIs effortlessly. Whether you want to retrieve player data, manage groups, or create dynamic game interactions, BloxPy empowers you to build amazing Roblox experiences with ease.
 
 [![License](https://img.shields.io/github/license/Developer-X-0001/BloxPy)](https://github.com/Developer-X-0001/BloxPy/blob/main/LICENSE)
 [![PyPI Version](https://img.shields.io/pypi/v/BloxPy)](https://pypi.org/project/BloxPy/)
 [![Python Version](https://img.shields.io/pypi/pyversions/BloxPy)](https://pypi.org/project/BloxPy/)
 
 ## Features
 
@@ -21,26 +21,58 @@
 
 ```bash
 pip install BloxPy
 ```
 
 ## Usage
 
+- ### Users
 ```py
-import BloxPy
+from BloxPy import Users
 
 # Fetch player data
 player_id = 1234567890
-player_data = BloxPy.get_player_data(player_id)
-print(player_data)
+player_data = Users.get_user(player_id)
+print(player_data.name) # Username
+print(player_data.displayName) # Display Name
+```
+
+- ### Groups
+```py
+from BloxPy import Groups
+
+# Fetch group data
+group_id = 1234567890
+group_data = Groups.get_group(group_id)
+print(group_data.name) # Group Name
+print(group_data.memberCount) # Group Member Count
+```
+
+- ### Search
+```py
+from BloxPy import Search
 
-# Manage groups
-group_id = 9876543210
-group_members = BloxPy.get_group_members(group_id)
-print(group_members)
+# Fetch users by keyword
+user_keyword = 'Henry'
+user_search_results = Search.search_users(keyword)
+print(user_search_results.data) # List containing data
+
+for user in user_search_results.data:
+    print(user.name) # Username
+    print(user.id) # User ID
+
+# Fetch groups by keyword
+group_keyword = 'Roblox'
+group_search_results = Search.search_groups(keyword)
+print(group_search_results.data) # List containing data
+
+for group in group_search_results.data:
+    print(group.name) # Name
+    print(group.description) # Description
+    print(group.memberCount) # Member Count
 ```
 
 ## Documentation
 
 For detailed documentation and usage examples, check out the [BloxPy Documentation](https://Developer-X-0001.github.io/BloxPy-docs).
 
 ## Contributing
```

### Comparing `BloxPy-0.1.11/setup.py` & `BloxPy-0.1.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 NAME = 'BloxPy'
-VERSION = '0.1.11'
-DESCRIPTION = 'BloxPy: Your All-in-One Python Library for Roblox Development'
-LONG_DESCRIPTION = 'BloxPy is the ultimate Python library for Roblox developers, offering an all-in-one solution to interact with Roblox Public APIs effortlessly. Whether you want to retrieve player data, manage groups, or create dynamic game interactions, BloxPy empowers you to build amazing Roblox experiences with ease.'
+VERSION = '0.1.12'
+DESCRIPTION = 'BloxPy: Your All-in-One Python API wrapper for Roblox Development'
+LONG_DESCRIPTION = 'BloxPy is the ultimate Python API wrapper for Roblox developers, offering an all-in-one solution to interact with Roblox Public APIs effortlessly. Whether you want to retrieve player data, manage groups, or create dynamic game interactions, BloxPy empowers you to build amazing Roblox experiences with ease.'
 AUTHOR = 'Developer X'
 EMAIL = 'developer.x.business@gmail.com'
-URL = 'https://github.com/yourusername/bloxpy'
+URL = 'https://github.com/Developer-X-0001/BloxPy'
 LICENSE = 'MIT'
-PYTHON_REQUIRES = '>=3.6'
+PYTHON_REQUIRES = '>=3.9'
 
 with open('README.md', 'r', encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 REQUIRES = [
     'requests', 
 ]
```

