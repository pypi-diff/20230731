# Comparing `tmp/magnetocaloric-1.2.0.tar.gz` & `tmp/magnetocaloric-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnetocaloric-1.2.0.tar", last modified: Thu Jul 27 08:36:41 2023, max compression
+gzip compressed data, was "magnetocaloric-1.2.1.tar", last modified: Mon Jul 31 06:25:36 2023, max compression
```

## Comparing `magnetocaloric-1.2.0.tar` & `magnetocaloric-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 08:36:41.118427 magnetocaloric-1.2.0/
--rw-rw-rw-   0        0        0       84 2022-04-14 07:58:46.000000 magnetocaloric-1.2.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-27 08:24:00.000000 magnetocaloric-1.2.0/Licence.txt
--rw-rw-rw-   0        0        0       81 2022-04-14 07:58:45.000000 magnetocaloric-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4467 2023-07-27 08:36:41.118427 magnetocaloric-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3720 2023-07-27 08:22:32.000000 magnetocaloric-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 08:36:41.102798 magnetocaloric-1.2.0/magnetocaloric/
--rw-rw-rw-   0        0        0    15967 2023-07-27 07:04:32.000000 magnetocaloric-1.2.0/magnetocaloric/__init__.py
--rw-rw-rw-   0        0        0    15967 2023-07-27 07:02:01.000000 magnetocaloric-1.2.0/magnetocaloric/mcepy.py
-drwxrwxrwx   0        0        0        0 2023-07-27 08:36:41.118427 magnetocaloric-1.2.0/magnetocaloric.egg-info/
--rw-rw-rw-   0        0        0     4467 2023-07-27 08:36:40.000000 magnetocaloric-1.2.0/magnetocaloric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-27 08:36:40.000000 magnetocaloric-1.2.0/magnetocaloric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 08:36:40.000000 magnetocaloric-1.2.0/magnetocaloric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-07-27 08:36:40.000000 magnetocaloric-1.2.0/magnetocaloric.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-27 08:36:40.000000 magnetocaloric-1.2.0/magnetocaloric.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 08:36:41.118427 magnetocaloric-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1180 2023-07-27 08:23:40.000000 magnetocaloric-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:25:36.596790 magnetocaloric-1.2.1/
+-rw-rw-rw-   0        0        0       84 2022-04-14 07:58:46.000000 magnetocaloric-1.2.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-27 08:24:00.000000 magnetocaloric-1.2.1/Licence.txt
+-rw-rw-rw-   0        0        0       81 2022-04-14 07:58:45.000000 magnetocaloric-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3969 2023-07-31 06:25:36.596790 magnetocaloric-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3222 2023-07-31 06:24:49.000000 magnetocaloric-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 06:25:36.565530 magnetocaloric-1.2.1/magnetocaloric/
+-rw-rw-rw-   0        0        0      560 2023-07-31 06:14:28.000000 magnetocaloric-1.2.1/magnetocaloric/Color_marker.py
+-rw-rw-rw-   0        0        0     1397 2023-07-30 11:40:32.000000 magnetocaloric-1.2.1/magnetocaloric/M_H_reshaping.py
+-rw-rw-rw-   0        0        0     2059 2023-07-30 11:43:59.000000 magnetocaloric-1.2.1/magnetocaloric/RCP_plot.py
+-rw-rw-rw-   0        0        0     3548 2023-07-30 11:43:19.000000 magnetocaloric-1.2.1/magnetocaloric/T_FWHM_RCP.py
+-rw-rw-rw-   0        0        0      831 2023-07-30 12:08:19.000000 magnetocaloric-1.2.1/magnetocaloric/__init__.py
+-rw-rw-rw-   0        0        0     1487 2023-07-30 11:41:26.000000 magnetocaloric-1.2.1/magnetocaloric/arrott_plot.py
+-rw-rw-rw-   0        0        0     1424 2023-07-30 11:37:12.000000 magnetocaloric-1.2.1/magnetocaloric/collect_from_database.py
+-rw-rw-rw-   0        0        0     5564 2023-07-31 06:14:23.000000 magnetocaloric-1.2.1/magnetocaloric/data_visualization.py
+-rw-rw-rw-   0        0        0     2433 2023-07-31 06:15:05.000000 magnetocaloric-1.2.1/magnetocaloric/entropy_change01.py
+-rw-rw-rw-   0        0        0     1229 2023-07-30 11:38:43.000000 magnetocaloric-1.2.1/magnetocaloric/entropy_change02.py
+-rw-rw-rw-   0        0        0     3943 2023-07-31 06:24:52.000000 magnetocaloric-1.2.1/magnetocaloric/mcepy.py
+-rw-rw-rw-   0        0        0     2434 2023-07-30 11:42:47.000000 magnetocaloric-1.2.1/magnetocaloric/modified_arrott_plot.py
+-rw-rw-rw-   0        0        0     2164 2023-07-30 11:39:58.000000 magnetocaloric-1.2.1/magnetocaloric/store_to_database.py
+-rw-rw-rw-   0        0        0      930 2023-07-30 11:36:24.000000 magnetocaloric-1.2.1/magnetocaloric/take_temp.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:25:36.596790 magnetocaloric-1.2.1/magnetocaloric.egg-info/
+-rw-rw-rw-   0        0        0     3969 2023-07-31 06:25:36.000000 magnetocaloric-1.2.1/magnetocaloric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-07-31 06:25:36.000000 magnetocaloric-1.2.1/magnetocaloric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 06:25:36.000000 magnetocaloric-1.2.1/magnetocaloric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-31 06:25:36.000000 magnetocaloric-1.2.1/magnetocaloric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-31 06:25:36.000000 magnetocaloric-1.2.1/magnetocaloric.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 06:25:36.596790 magnetocaloric-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2023-07-31 06:24:46.000000 magnetocaloric-1.2.1/setup.py
```

### Comparing `magnetocaloric-1.2.0/Licence.txt` & `magnetocaloric-1.2.1/Licence.txt`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.0/PKG-INFO` & `magnetocaloric-1.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnetocaloric
-Version: 1.2.0
+Version: 1.2.1
 Summary: Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python
 Home-page: https://github.com/supratimdasinfo/Magnetocaloric-Effect
 Author: Supratim Das
 Author-email: supratim0707@gmail.com
 License: MIT
 Keywords: magnetocaloric,mcepy,magnetic,programming,code,python,supratim,das,bhaskar,biswas,physics
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: Licence.txt
 
 
-# magnetocaloric 1.2.0
+# magnetocaloric 1.2.1
 #### Developed by Supratim Das
 
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
 
 Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
 
 ## What's New
@@ -38,15 +38,15 @@
 
 ### 1. Installation 
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
 
 ```bash
 
- pip install magnetocaloric==1.2.0
+ pip install magnetocaloric==1.2.1
 
 ```
 ### 2. Manage Excel Spreadsheet
 -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
 
 ![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
 
@@ -57,24 +57,28 @@
 - Create two new files (file extension xlsx) to hold the results obtained after the calculation and definitely make them closed, other wise XlsxWriter will not get access.
 
 ###  3. Execution
 Run the code at any python based environment ( IDLE, PyCharm, Spyder etc.). But I recommend you simply execute this code using command prompt or IDLE. 
 
 ```python
 
-import magnetocaloric.mcepy as mc
+from magnetocaloric import mcepy as mc
+
+# Assuming `a` and `b` are provided by the user
 mc.mce(a, b)
 
+
 ```
 Here, 'a' is the total number of temperature and 'b' is the total number of applied magnetic field.
 
 ## Contributing
 ### We Welcome Your Contributions!
 
 If you're interested in contributing to the development of this project, your contributions are highly appreciated. Whether you find a bug, have an idea for a new feature, or want to improve the code, you can do so by raising an issue or pull request on our GitHub repository. Your input helps make this project better for everyone.
 
 Feel free to explore the code, try out the application, and share your thoughts with us. We value the contributions of our community members and look forward to collaborating with you. Let's make this project even more amazing together!
 
+### Contact Information: 
+
+If you have any questions or need assistance, you can reach out to me directly via email at supratim0707@gmail.com.
 
-## Caution
 
-- Before adding the Hmax + del_H value into the M(H) spreadsheet, The maximum value of applied magnetic field (Hmax) must be the multiple of (10xdel_H). As an example, if del_H = 500 Oe / 0.05 T, Hmax must be like 5000 Oe/0.5 T, 10000 Oe / 1 T, 15000 Oe / 1.5 T,........ or any other multiple of (10x500 Oe) whether the value of the magnetic field is Tesla or Oersted. For another example, if del_H = 700 Oe / 0.07 T, Hmax must be like 7000 Oe/0.7 T, 14000 Oe / 1.4 T, 21000 Oe / 2.1 T,........ or any other multiple of (10x700 Oe). Otherwise Hmax for not being a proper numbered figure, an error may occur. This caution is also applicable to the previous versions of the package as well.
```

### Comparing `magnetocaloric-1.2.0/README.md` & `magnetocaloric-1.2.1/magnetocaloric.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,26 @@
+Metadata-Version: 2.1
+Name: magnetocaloric
+Version: 1.2.1
+Summary: Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python
+Home-page: https://github.com/supratimdasinfo/Magnetocaloric-Effect
+Author: Supratim Das
+Author-email: supratim0707@gmail.com
+License: MIT
+Keywords: magnetocaloric,mcepy,magnetic,programming,code,python,supratim,das,bhaskar,biswas,physics
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Education
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: Licence.txt
 
-# magnetocaloric 1.2.0
+
+# magnetocaloric 1.2.1
 #### Developed by Supratim Das
 
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
 
 Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
 
 ## What's New
@@ -21,15 +38,15 @@
 
 ### 1. Installation 
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
 
 ```bash
 
- pip install magnetocaloric==1.2.0
+ pip install magnetocaloric==1.2.1
 
 ```
 ### 2. Manage Excel Spreadsheet
 -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
 
 ![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
 
@@ -40,24 +57,28 @@
 - Create two new files (file extension xlsx) to hold the results obtained after the calculation and definitely make them closed, other wise XlsxWriter will not get access.
 
 ###  3. Execution
 Run the code at any python based environment ( IDLE, PyCharm, Spyder etc.). But I recommend you simply execute this code using command prompt or IDLE. 
 
 ```python
 
-import magnetocaloric.mcepy as mc
+from magnetocaloric import mcepy as mc
+
+# Assuming `a` and `b` are provided by the user
 mc.mce(a, b)
 
+
 ```
 Here, 'a' is the total number of temperature and 'b' is the total number of applied magnetic field.
 
 ## Contributing
 ### We Welcome Your Contributions!
 
 If you're interested in contributing to the development of this project, your contributions are highly appreciated. Whether you find a bug, have an idea for a new feature, or want to improve the code, you can do so by raising an issue or pull request on our GitHub repository. Your input helps make this project better for everyone.
 
 Feel free to explore the code, try out the application, and share your thoughts with us. We value the contributions of our community members and look forward to collaborating with you. Let's make this project even more amazing together!
 
+### Contact Information: 
+
+If you have any questions or need assistance, you can reach out to me directly via email at supratim0707@gmail.com.
 
-## Caution
 
-- Before adding the Hmax + del_H value into the M(H) spreadsheet, The maximum value of applied magnetic field (Hmax) must be the multiple of (10xdel_H). As an example, if del_H = 500 Oe / 0.05 T, Hmax must be like 5000 Oe/0.5 T, 10000 Oe / 1 T, 15000 Oe / 1.5 T,........ or any other multiple of (10x500 Oe) whether the value of the magnetic field is Tesla or Oersted. For another example, if del_H = 700 Oe / 0.07 T, Hmax must be like 7000 Oe/0.7 T, 14000 Oe / 1.4 T, 21000 Oe / 2.1 T,........ or any other multiple of (10x700 Oe). Otherwise Hmax for not being a proper numbered figure, an error may occur. This caution is also applicable to the previous versions of the package as well.
```

### Comparing `magnetocaloric-1.2.0/setup.py` & `magnetocaloric-1.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='magnetocaloric',
-  version='1.2.0',
+  version='1.2.1',
   description='Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python',
   long_description=long_description,
   long_description_content_type="text/markdown",
   url='https://github.com/supratimdasinfo/Magnetocaloric-Effect',  
   author='Supratim Das',
   author_email='supratim0707@gmail.com',
   license='MIT',
```

