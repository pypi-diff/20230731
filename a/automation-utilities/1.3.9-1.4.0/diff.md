# Comparing `tmp/automation-utilities-1.3.9.tar.gz` & `tmp/automation-utilities-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-utilities-1.3.9.tar", last modified: Fri Jul 21 18:11:34 2023, max compression
+gzip compressed data, was "automation-utilities-1.4.0.tar", last modified: Mon Jul 31 01:13:11 2023, max compression
```

## Comparing `automation-utilities-1.3.9.tar` & `automation-utilities-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 18:11:34.689264 automation-utilities-1.3.9/
-drwxrwxrwx   0        0        0        0 2023-07-21 18:11:34.684251 automation-utilities-1.3.9/Automation_Utilities.egg-info/
--rw-rw-rw-   0        0        0      134 2023-07-21 18:11:34.000000 automation-utilities-1.3.9/Automation_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      694 2023-07-21 18:11:34.000000 automation-utilities-1.3.9/Automation_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 18:11:34.000000 automation-utilities-1.3.9/Automation_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-21 18:11:34.000000 automation-utilities-1.3.9/Automation_Utilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-21 18:11:34.000000 automation-utilities-1.3.9/Automation_Utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-07-21 18:11:34.689264 automation-utilities-1.3.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 18:11:34.678762 automation-utilities-1.3.9/automation_utilities/
--rw-rw-rw-   0        0        0      186 2023-07-19 17:03:31.000000 automation-utilities-1.3.9/automation_utilities/Control.py
--rw-rw-rw-   0        0        0     1575 2023-07-20 11:40:18.000000 automation-utilities-1.3.9/automation_utilities/Data.py
--rw-rw-rw-   0        0        0       82 2023-07-20 19:25:23.000000 automation-utilities-1.3.9/automation_utilities/Exceptions.py
--rw-rw-rw-   0        0        0      936 2023-07-18 19:42:13.000000 automation-utilities-1.3.9/automation_utilities/Files.py
--rw-rw-rw-   0        0        0        0 2023-07-20 19:11:30.000000 automation-utilities-1.3.9/automation_utilities/Generator.py
--rw-rw-rw-   0        0        0      147 2023-07-02 15:43:12.000000 automation-utilities-1.3.9/automation_utilities/Input.py
--rw-rw-rw-   0        0        0      835 2023-06-27 20:34:27.000000 automation-utilities-1.3.9/automation_utilities/PhoneNumbers.py
--rw-rw-rw-   0        0        0      525 2023-07-20 19:11:30.000000 automation-utilities-1.3.9/automation_utilities/__init__.py
--rw-rw-rw-   0        0        0     2195 2023-07-21 18:11:32.000000 automation-utilities-1.3.9/automation_utilities/mailtm.py
--rw-rw-rw-   0        0        0       42 2023-07-21 18:11:34.689264 automation-utilities-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0      307 2023-07-21 18:11:32.000000 automation-utilities-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:13:11.734111 automation-utilities-1.4.0/
+drwxrwxrwx   0        0        0        0 2023-07-31 01:13:11.731839 automation-utilities-1.4.0/Automation_Utilities.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-07-31 01:13:10.000000 automation-utilities-1.4.0/Automation_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      726 2023-07-31 01:13:10.000000 automation-utilities-1.4.0/Automation_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 01:13:10.000000 automation-utilities-1.4.0/Automation_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-31 01:13:10.000000 automation-utilities-1.4.0/Automation_Utilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-31 01:13:10.000000 automation-utilities-1.4.0/Automation_Utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-07-31 01:13:11.732969 automation-utilities-1.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-31 01:13:11.723885 automation-utilities-1.4.0/automation_utilities/
+-rw-rw-rw-   0        0        0      186 2023-07-19 17:03:31.000000 automation-utilities-1.4.0/automation_utilities/Control.py
+-rw-rw-rw-   0        0        0     1628 2023-07-28 20:33:25.000000 automation-utilities-1.4.0/automation_utilities/Data.py
+-rw-rw-rw-   0        0        0       82 2023-07-20 19:25:23.000000 automation-utilities-1.4.0/automation_utilities/Exceptions.py
+-rw-rw-rw-   0        0        0      936 2023-07-18 19:42:13.000000 automation-utilities-1.4.0/automation_utilities/Files.py
+-rw-rw-rw-   0        0        0     1918 2023-07-30 08:46:44.000000 automation-utilities-1.4.0/automation_utilities/FiveSim.py
+-rw-rw-rw-   0        0        0        0 2023-07-20 19:11:30.000000 automation-utilities-1.4.0/automation_utilities/Generator.py
+-rw-rw-rw-   0        0        0      147 2023-07-02 15:43:12.000000 automation-utilities-1.4.0/automation_utilities/Input.py
+-rw-rw-rw-   0        0        0      835 2023-06-27 20:34:27.000000 automation-utilities-1.4.0/automation_utilities/PhoneNumbers.py
+-rw-rw-rw-   0        0        0      525 2023-07-20 19:11:30.000000 automation-utilities-1.4.0/automation_utilities/__init__.py
+-rw-rw-rw-   0        0        0     2195 2023-07-21 18:11:32.000000 automation-utilities-1.4.0/automation_utilities/mailtm.py
+-rw-rw-rw-   0        0        0       42 2023-07-31 01:13:11.734111 automation-utilities-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      307 2023-07-31 01:13:06.000000 automation-utilities-1.4.0/setup.py
```

### Comparing `automation-utilities-1.3.9/Automation_Utilities.egg-info/SOURCES.txt` & `automation-utilities-1.4.0/Automation_Utilities.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Automation_Utilities.egg-info/SOURCES.txt
 Automation_Utilities.egg-info/dependency_links.txt
 Automation_Utilities.egg-info/top_level.txt
 automation_utilities/Control.py
 automation_utilities/Data.py
 automation_utilities/Exceptions.py
 automation_utilities/Files.py
+automation_utilities/FiveSim.py
 automation_utilities/Generator.py
 automation_utilities/Input.py
 automation_utilities/PhoneNumbers.py
 automation_utilities/__init__.py
 automation_utilities/mailtm.py
 automation_utilities.egg-info/PKG-INFO
 automation_utilities.egg-info/SOURCES.txt
```

### Comparing `automation-utilities-1.3.9/automation_utilities/Data.py` & `automation-utilities-1.4.0/automation_utilities/Data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import json
 import threading
+from json import JSONDecodeError
 
 
 class Data:
     lock = threading.Lock()
 
     def __init__(self, file_name: str):
         self.file_name = file_name
         try:
             self.data = json.load(open(file_name, 'r', encoding='utf-8'))
-        except FileNotFoundError:
+        except (FileNotFoundError, JSONDecodeError):
             self.data = {}
         self._privte = 15
 
     def __call__(self, key, from_list: list = None, loop: bool = False):
         return self.get(key, from_list, loop)
 
     def get(self, key, from_list: list = None, loop: bool = False):
```

### Comparing `automation-utilities-1.3.9/automation_utilities/Files.py` & `automation-utilities-1.4.0/automation_utilities/Files.py`

 * *Files identical despite different names*

### Comparing `automation-utilities-1.3.9/automation_utilities/PhoneNumbers.py` & `automation-utilities-1.4.0/automation_utilities/PhoneNumbers.py`

 * *Files identical despite different names*

### Comparing `automation-utilities-1.3.9/automation_utilities/__init__.py` & `automation-utilities-1.4.0/automation_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `automation-utilities-1.3.9/automation_utilities/mailtm.py` & `automation-utilities-1.4.0/automation_utilities/mailtm.py`

 * *Files identical despite different names*

