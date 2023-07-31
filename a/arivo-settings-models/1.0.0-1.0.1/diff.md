# Comparing `tmp/arivo-settings_models-1.0.0.tar.gz` & `tmp/arivo-settings_models-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arivo-settings_models-1.0.0.tar", last modified: Tue Jul 25 12:50:00 2023, max compression
+gzip compressed data, was "dist/arivo-settings_models-1.0.1.tar", last modified: Mon Jul 31 09:04:36 2023, max compression
```

## Comparing `arivo-settings_models-1.0.0.tar` & `arivo-settings_models-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1353 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/docs/migrations.md
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/test-requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      704 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/tools/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/tools/pages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      704 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      922 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/.coveragerc
--rw-r--r--   0 root         (0) root         (0)      111 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     1433 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/ChangeLog
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)    38906 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/tests/test_validation.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11501 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     3417 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/tests/test_serialization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/settings_models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6344 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/_combat.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/doc.py
--rw-rw-rw-   0 root         (0) root         (0)     1977 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/settings_models/settings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/settings/enforcement.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/settings/device_keys.py
--rw-rw-rw-   0 root         (0) root         (0)    20512 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/settings/common.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/settings/intercom.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/settings/gate_control.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/docs/migrations.md
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/test-requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      704 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/tools/pages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      704 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      922 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/arivo_settings_models.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/ChangeLog
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    39686 2023-07-31 09:04:25.000000 arivo-settings_models-1.0.1/tests/test_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11501 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3417 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/tests/test_serialization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/settings_models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 09:04:25.000000 arivo-settings_models-1.0.1/settings_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6344 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/_combat.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/doc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1977 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 09:04:36.000000 arivo-settings_models-1.0.1/settings_models/settings/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 09:04:25.000000 arivo-settings_models-1.0.1/settings_models/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/settings/enforcement.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/settings/device_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    21017 2023-07-31 09:04:25.000000 arivo-settings_models-1.0.1/settings_models/settings/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/settings/intercom.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.1/settings_models/settings/gate_control.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.1/tox.ini
```

### Comparing `arivo-settings_models-1.0.0/.gitlab-ci.yml` & `arivo-settings_models-1.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.0/PKG-INFO` & `arivo-settings_models-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arivo-settings_models
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library for arivo parking system settings definitions and models
 Home-page: https://gitlab.com/accessio/onegate/settings-models
 Author: ARIVO
 Author-email: support@arivo.co
 License: "GPL-3",
 Description: # Settings Models
```

### Comparing `arivo-settings_models-1.0.0/arivo_settings_models.egg-info/PKG-INFO` & `arivo-settings_models-1.0.1/arivo_settings_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arivo-settings-models
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library for arivo parking system settings definitions and models
 Home-page: https://gitlab.com/accessio/onegate/settings-models
 Author: ARIVO
 Author-email: support@arivo.co
 License: "GPL-3",
 Description: # Settings Models
```

### Comparing `arivo-settings_models-1.0.0/arivo_settings_models.egg-info/SOURCES.txt` & `arivo-settings_models-1.0.1/arivo_settings_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.0/ChangeLog` & `arivo-settings_models-1.0.1/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+v1.0.1
+------
+
+* changes in support setting
+
 v1.0.0
 ------
 
 * parking areas: default cost entries requires shortterm gates
 
 v0.0.1rc4
 ---------
@@ -63,8 +68,7 @@
 v0.0.0rc0
 ---------
 
 * added testcase for refs
 * coverage fix
 * removing pages stage because no documentation yet
 * settings models and parsing/serializing
-* committing before weekend [skip ci]
```

### Comparing `arivo-settings_models-1.0.0/setup.cfg` & `arivo-settings_models-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.0/tests/test_validation.py` & `arivo-settings_models-1.0.1/tests/test_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -503,19 +503,34 @@
 
     def test_support_success(self):
         gt = dump_setting({
             "name": "Test", "address": {
                 "name": "Garage", "street": "Garagestreet", "number": "12c",
                 "floor": "2H", "door": "7a", "supplements": "Frag nach Ines", "city": "Graz",
                 "zip_code": "8020", "state": "Styria", "country": "Österreich"},
-            "phone_number": "+43 123 456 789", "email_address": "ines@arivo.co"
+            "phone_number": "+43 123 456 789", "email_address": "ines@arivo.co", "website": "https://arivo.co/support"
         })
         res = parse_setting("common/support", gt)
         self.assert_result(res, gt)
 
+    def test_support_not_given(self):
+        gt = dump_setting({"name": "Test", "phone_number": "+43 123 456 789"})
+        res = parse_setting("common/support", gt)
+        self.assert_result(res, gt)
+        gt = dump_setting({"name": "Test", "website": "https://arivo.co"})
+        res = parse_setting("common/support", gt)
+        self.assert_result(res, gt)
+
+        with self.assertRaises(ValidationError) as e:
+            gt = dump_setting({"name": "Test"})
+            res = parse_setting("common/support", gt)
+            self.assert_result(res, gt)
+        self.assertEqual(str(e.exception).count("\n"), 2)
+        self.assertIn("At least one of address, phone_number, email_address or website must be given", str(e.exception))
+
     def test_support_invalid_email(self):
         with self.assertRaises(ValidationError) as e:
             parse_setting("common/support", dump_setting({
                 "name": "Test", "address": {
                     "name": "Garage", "street": "Garagestreet", "number": "12c",
                     "floor": "2H", "door": "7a", "supplements": "Frag nach Ines", "city": "Graz",
                     "zip_code": "8020", "state": "Styria", "country": "Österreich"},
```

### Comparing `arivo-settings_models-1.0.0/tests/utils.py` & `arivo-settings_models-1.0.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.0/tests/test_models.py` & `arivo-settings_models-1.0.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.0/tests/test_serialization.py` & `arivo-settings_models-1.0.1/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.0/settings_models/serialization.py` & `arivo-settings_models-1.0.1/settings_models/serialization.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.0/settings_models/validators.py` & `arivo-settings_models-1.0.1/settings_models/validators.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.0/settings_models/settings/device_keys.py` & `arivo-settings_models-1.0.1/settings_models/settings/device_keys.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-1.0.0/settings_models/settings/common.py` & `arivo-settings_models-1.0.1/settings_models/settings/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,19 +340,27 @@
 class SupportSettings(SettingsModel):
     """
     Contact data for support cases (e.g. shown at signs, displays or end user UIs).
     Support means questions to contracts or complaints against costs and NOT emergency calls
     (cannot enter door, cannot pay, ...)
     """
     name: str = Field(..., description="Name of the person/entity responsible for support, e.g. provider")
-    address: AddressModel = Field(..., description="Address for written support letters")
-    phone_number: constr(min_length=3, max_length=32, regex=r"^\+[0-9 ]+$") = \
-        Field(..., description="Phone number for support (not emergency calls)")
-    email_address: constr(min_length=3, max_length=254, regex=r"^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$") = \
-        Field(..., description="Email address for support")
+    address: Optional[AddressModel] = Field(None, description="Address for written support letters")
+    phone_number: Optional[constr(min_length=3, max_length=32, regex=r"^\+[0-9 ]+$")] = \
+        Field(None, description="Phone number for support (not emergency calls)")
+    email_address: Optional[constr(min_length=3, max_length=254,
+                                   regex=r"^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$")] = \
+        Field(None, description="Email address for support")
+    website: Optional[constr(min_length=3, max_length=1022)] = Field(None, description="Website for support")
+
+    @root_validator(skip_on_failure=True)
+    def data_validation(cls, values):
+        if (values["address"] or values["phone_number"] or values["email_address"] or values["website"]) is None:
+            raise ValueError("At least one of address, phone_number, email_address or website must be given")
+        return values
 
 
 class GarageModes(str, Enum):
     """
     Garage modes
     """
     barrier = "barrier"
```

### Comparing `arivo-settings_models-1.0.0/settings_models/settings/gate_control.py` & `arivo-settings_models-1.0.1/settings_models/settings/gate_control.py`

 * *Files identical despite different names*

