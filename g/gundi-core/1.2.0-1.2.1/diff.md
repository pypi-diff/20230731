# Comparing `tmp/gundi_core-1.2.0.tar.gz` & `tmp/gundi_core-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gundi_core-1.2.0.tar", max compression
+gzip compressed data, was "gundi_core-1.2.1.tar", max compression
```

## Comparing `gundi_core-1.2.0.tar` & `gundi_core-1.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       40 2023-06-14 17:07:47.722189 gundi_core-1.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-14 20:35:09.913772 gundi_core-1.2.0/gundi_core/__init__.py
--rw-r--r--   0        0        0       47 2023-07-07 19:55:59.544656 gundi_core-1.2.0/gundi_core/events/__init__.py
--rw-r--r--   0        0        0     1019 2023-07-10 15:33:44.398106 gundi_core-1.2.0/gundi_core/events/core.py
--rw-r--r--   0        0        0      308 2023-07-07 18:45:50.769675 gundi_core-1.2.0/gundi_core/events/dispatchers.py
--rw-r--r--   0        0        0      114 2023-06-14 18:33:55.875739 gundi_core-1.2.0/gundi_core/schemas/__init__.py
--rw-r--r--   0        0        0    13847 2023-06-14 19:41:05.310697 gundi_core-1.2.0/gundi_core/schemas/v1.py
--rw-r--r--   0        0        0    14678 2023-07-14 12:24:28.304354 gundi_core-1.2.0/gundi_core/schemas/v2.py
--rw-r--r--   0        0        0      329 2023-07-14 12:15:33.494447 gundi_core-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 gundi_core-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       40 2023-06-14 17:07:47.722189 gundi_core-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 20:35:09.913772 gundi_core-1.2.1/gundi_core/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-31 13:14:26.547739 gundi_core-1.2.1/gundi_core/events/__init__.py
+-rw-r--r--   0        0        0     1019 2023-07-31 13:14:26.547739 gundi_core-1.2.1/gundi_core/events/core.py
+-rw-r--r--   0        0        0      308 2023-07-31 13:14:26.547739 gundi_core-1.2.1/gundi_core/events/dispatchers.py
+-rw-r--r--   0        0        0      114 2023-06-14 18:33:55.875739 gundi_core-1.2.1/gundi_core/schemas/__init__.py
+-rw-r--r--   0        0        0    13847 2023-06-14 19:41:05.310697 gundi_core-1.2.1/gundi_core/schemas/v1.py
+-rw-r--r--   0        0        0    15633 2023-07-31 13:14:26.799749 gundi_core-1.2.1/gundi_core/schemas/v2.py
+-rw-r--r--   0        0        0      330 2023-07-31 13:14:43.600428 gundi_core-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 gundi_core-1.2.1/PKG-INFO
```

### Comparing `gundi_core-1.2.0/gundi_core/events/core.py` & `gundi_core-1.2.1/gundi_core/events/core.py`

 * *Files identical despite different names*

### Comparing `gundi_core-1.2.0/gundi_core/schemas/v1.py` & `gundi_core-1.2.1/gundi_core/schemas/v1.py`

 * *Files identical despite different names*

### Comparing `gundi_core-1.2.0/gundi_core/schemas/v2.py` & `gundi_core-1.2.1/gundi_core/schemas/v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,30 +124,58 @@
     description: Optional[str] = Field(
         "",
         example="An organization in X dedicated to protect YZ..",
         description="Description of the organization owning this connection",
     )
 
 
+class ConnectionIntegrationType(BaseModel):
+    id: Union[UUID, str] = Field(
+        None,
+        title="Integration Type ID",
+        description="Id of an integration in Gundi",
+    )
+    name: Optional[str] = Field(
+        "",
+        example="EarthRanger",
+        description="Name of the third-party system or technology",
+    )
+    value: Optional[str] = Field(
+        "",
+        example="earth_ranger",
+        description="Natural key for the technology type",
+    )
+
+
+class ConnectionIntegrationOwner(BaseModel):
+    id: Union[UUID, str] = Field(
+        None,
+        title="Organization ID",
+        description="Id of the organization owning the connection",
+    )
+    name: Optional[str] = Field(
+        "",
+        example="Wild Conservation Organization X",
+        description="Name of the organization owning this connection",
+    )
+
+
 class ConnectionIntegration(BaseModel):
     id: Union[UUID, str] = Field(
         None,
         title="Integration ID",
         description="Id of an integration associated to the connection",
     )
     name: Optional[str] = Field(
         "",
         example="X Data Provider for Y Reserve",
         description="Connection name (Data Provider)",
     )
-    type: Optional[str] = Field(
-        "",
-        example="earth_ranger",
-        description="natural key of an integration type",
-    )
+    type: Optional[ConnectionIntegrationType]
+    owner: Optional[ConnectionIntegrationOwner]
     base_url: Optional[str] = Field(
         "",
         example="https://easterisland.pamdas.org/",
         description="Base URL of the third party system associated with this integration.",
     )
     status: Optional[str] = Field(
         "unknown",
@@ -283,14 +311,19 @@
         description="Id of an integration in Gundi",
     )
     name: Optional[str] = Field(
         "",
         example="EarthRanger",
         description="Name of the third-party system or technology",
     )
+    value: Optional[str] = Field(
+        "",
+        example="earth_ranger",
+        description="Natural key for the technology type",
+    )
     description: Optional[str] = Field(
         "",
         example="EarthRanger is a software solution for wildlife monitoring and protection in real-time.",
         description="Description of the third-party system or technology",
     )
     actions: Optional[List[IntegrationAction]]
```

### Comparing `gundi_core-1.2.0/PKG-INFO` & `gundi_core-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gundi-core
-Version: 1.2.0
+Version: 1.2.1
 Summary: 
 Author: Mariano M
 Author-email: marianom@earthranger.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

