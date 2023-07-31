# Comparing `tmp/ansys-api-discovery-0.4.1.tar.gz` & `tmp/ansys-api-discovery-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-discovery-0.4.1.tar", last modified: Wed Apr 19 07:08:23 2023, max compression
+gzip compressed data, was "ansys-api-discovery-0.4.2.tar", last modified: Mon Jul 31 06:13:26 2023, max compression
```

## Comparing `ansys-api-discovery-0.4.1.tar` & `ansys-api-discovery-0.4.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:08:23.939398 ansys-api-discovery-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-19 07:08:23.935398 ansys-api-discovery-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:08:23.931397 ansys-api-discovery-0.4.1/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:08:23.931397 ansys-api-discovery-0.4.1/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:08:23.935398 ansys-api-discovery-0.4.1/ansys/api/discovery/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:08:23.935398 ansys-api-discovery-0.4.1/ansys/api/discovery/v0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/v0/admintools.proto
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/v0/datamodels.proto
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/v0/definedvariationstable.proto
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/v0/discoveryapi.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/v0/discoveryapplication.proto
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/v0/discoverystreaming.proto
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/v0/documents.proto
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/v0/drivingdimensions.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/v0/historytrackparameters.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/v0/scriptparameters.proto
--rw-r--r--   0 runner    (1001) docker     (123)    45440 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/v0/units.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/ansys/api/discovery/v0/windows.proto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:08:23.935398 ansys-api-discovery-0.4.1/ansys_api_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-19 07:08:23.000000 ansys-api-discovery-0.4.1/ansys_api_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-19 07:08:23.000000 ansys-api-discovery-0.4.1/ansys_api_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 07:08:23.000000 ansys-api-discovery-0.4.1/ansys_api_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-19 07:08:23.000000 ansys-api-discovery-0.4.1/ansys_api_discovery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 07:08:23.000000 ansys-api-discovery-0.4.1/ansys_api_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 07:08:23.000000 ansys-api-discovery-0.4.1/ansys_api_discovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 07:08:23.939398 ansys-api-discovery-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-19 07:07:59.000000 ansys-api-discovery-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:13:26.606609 ansys-api-discovery-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-31 06:13:26.606609 ansys-api-discovery-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:13:26.602609 ansys-api-discovery-0.4.2/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:13:26.602609 ansys-api-discovery-0.4.2/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:13:26.606609 ansys-api-discovery-0.4.2/ansys/api/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:13:26.606609 ansys-api-discovery-0.4.2/ansys/api/discovery/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/v0/admintools.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/v0/datamodels.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/v0/definedvariationstable.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/v0/discoveryapi.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/v0/discoveryapplication.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/v0/discoverystreaming.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/v0/documents.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/v0/drivingdimensions.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/v0/historytrackparameters.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/v0/scriptparameters.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    45440 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/v0/units.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/ansys/api/discovery/v0/windows.proto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:13:26.606609 ansys-api-discovery-0.4.2/ansys_api_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-31 06:13:26.000000 ansys-api-discovery-0.4.2/ansys_api_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-31 06:13:26.000000 ansys-api-discovery-0.4.2/ansys_api_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:13:26.000000 ansys-api-discovery-0.4.2/ansys_api_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-31 06:13:26.000000 ansys-api-discovery-0.4.2/ansys_api_discovery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 06:13:26.000000 ansys-api-discovery-0.4.2/ansys_api_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 06:13:26.000000 ansys-api-discovery-0.4.2/ansys_api_discovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:13:26.606609 ansys-api-discovery-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-31 06:13:07.000000 ansys-api-discovery-0.4.2/setup.py
```

### Comparing `ansys-api-discovery-0.4.1/LICENSE` & `ansys-api-discovery-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.4.1/PKG-INFO` & `ansys-api-discovery-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: ansys-api-discovery
-Version: 0.4.1
-Summary: Autogenerated python gRPC interface package for ansys-api-discovery, built on 07:08:23 on 19 April 2023
+Version: 0.4.2
+Summary: Autogenerated python gRPC interface package for ansys-api-discovery, built on 06:13:26 on 31 July 2023
 Home-page: https://github.com/ansys/ansys-api-discovery
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### ansys-api-discovery gRPC Interface Package
 
-This repository provides the auto-generated gRPC Python interface files and NuGet
-packages for Discovery/SpaceClaim.
+This repository provides the auto-generated gRPC Python interface files
+for Discovery/SpaceClaim.
 
 
 #### Installation
 
 Provided that these wheels have been published to public PyPI, they can be
 installed with:
 
 ```
 pip install ansys-api-discovery
 ```
 
-Otherwise, see the
-
 
 #### Build
 
 To build the gRPC packages, run:
 
 ```
 pip install build
```

### Comparing `ansys-api-discovery-0.4.1/README.md` & `ansys-api-discovery-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 ### ansys-api-discovery gRPC Interface Package
 
-This repository provides the auto-generated gRPC Python interface files and NuGet
-packages for Discovery/SpaceClaim.
+This repository provides the auto-generated gRPC Python interface files
+for Discovery/SpaceClaim.
 
 
 #### Installation
 
 Provided that these wheels have been published to public PyPI, they can be
 installed with:
 
 ```
 pip install ansys-api-discovery
 ```
 
-Otherwise, see the
-
 
 #### Build
 
 To build the gRPC packages, run:
 
 ```
 pip install build
```

### Comparing `ansys-api-discovery-0.4.1/ansys/api/discovery/v0/admintools.proto` & `ansys-api-discovery-0.4.2/ansys/api/discovery/v0/admintools.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.4.1/ansys/api/discovery/v0/datamodels.proto` & `ansys-api-discovery-0.4.2/ansys/api/discovery/v0/datamodels.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.4.1/ansys/api/discovery/v0/definedvariationstable.proto` & `ansys-api-discovery-0.4.2/ansys/api/discovery/v0/definedvariationstable.proto`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   // Get an input variation table's cell
   rpc GetInputForVariation(GetInputForVariationRequest) returns(InputParameter);
     
   // Set an input parameter
   rpc SetInputValue(SetInputValueRequest) returns(InputParameter) ;
 
   // Create variation
-  rpc CreateVariation(CreateVariationRequest) returns(CreateVariationResponse);
+  rpc CreateVariation(google.protobuf.Empty) returns(Variation);
     
   // Get an output variation table's cell
   rpc GetOutputForVariation(GetOutputForVariationRequest) returns(OutputParameter);
     
   // Get a variation input table's column
   rpc GetInputColumn(GetInputColumnRequest) returns(GetInputColumnResponse);
     
@@ -117,21 +117,14 @@
 message SetStarredStatusRequest{
   // The variations monikers.
   repeated string variations_monikers = 1;
   // The starred status
   bool starred = 2;
 }
 
-message CreateVariationRequest{
-  string name= 1;
-}
-
-message CreateVariationResponse{
-  string result = 1;
-}
 ///UPDATES
 //
 
 message UpdateResponse{
   // The result
   bool result = 1;
 }
```

### Comparing `ansys-api-discovery-0.4.1/ansys/api/discovery/v0/discoveryapi.proto` & `ansys-api-discovery-0.4.2/ansys/api/discovery/v0/discoveryapi.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.4.1/ansys/api/discovery/v0/discoveryapplication.proto` & `ansys-api-discovery-0.4.2/ansys/api/discovery/v0/discoveryapplication.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.4.1/ansys/api/discovery/v0/documents.proto` & `ansys-api-discovery-0.4.2/ansys/api/discovery/v0/documents.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.4.1/ansys/api/discovery/v0/drivingdimensions.proto` & `ansys-api-discovery-0.4.2/ansys/api/discovery/v0/drivingdimensions.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.4.1/ansys/api/discovery/v0/historytrackparameters.proto` & `ansys-api-discovery-0.4.2/ansys/api/discovery/v0/historytrackparameters.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.4.1/ansys/api/discovery/v0/scriptparameters.proto` & `ansys-api-discovery-0.4.2/ansys/api/discovery/v0/scriptparameters.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.4.1/ansys/api/discovery/v0/units.proto` & `ansys-api-discovery-0.4.2/ansys/api/discovery/v0/units.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.4.1/ansys/api/discovery/v0/windows.proto` & `ansys-api-discovery-0.4.2/ansys/api/discovery/v0/windows.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.4.1/ansys_api_discovery.egg-info/PKG-INFO` & `ansys-api-discovery-0.4.2/ansys_api_discovery.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: ansys-api-discovery
-Version: 0.4.1
-Summary: Autogenerated python gRPC interface package for ansys-api-discovery, built on 07:08:23 on 19 April 2023
+Version: 0.4.2
+Summary: Autogenerated python gRPC interface package for ansys-api-discovery, built on 06:13:26 on 31 July 2023
 Home-page: https://github.com/ansys/ansys-api-discovery
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### ansys-api-discovery gRPC Interface Package
 
-This repository provides the auto-generated gRPC Python interface files and NuGet
-packages for Discovery/SpaceClaim.
+This repository provides the auto-generated gRPC Python interface files
+for Discovery/SpaceClaim.
 
 
 #### Installation
 
 Provided that these wheels have been published to public PyPI, they can be
 installed with:
 
 ```
 pip install ansys-api-discovery
 ```
 
-Otherwise, see the
-
 
 #### Build
 
 To build the gRPC packages, run:
 
 ```
 pip install build
```

### Comparing `ansys-api-discovery-0.4.1/ansys_api_discovery.egg-info/SOURCES.txt` & `ansys-api-discovery-0.4.2/ansys_api_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansys-api-discovery-0.4.1/setup.py` & `ansys-api-discovery-0.4.2/setup.py`

 * *Files identical despite different names*

