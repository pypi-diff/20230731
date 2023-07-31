# Comparing `tmp/threemystic_cloud_client-0.1.54.tar.gz` & `tmp/threemystic_cloud_client-0.1.55.tar.gz`

## Comparing `threemystic_cloud_client-0.1.54.tar` & `threemystic_cloud_client-0.1.55.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cli/actions/action_generate/__init__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cli/actions/action_test/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cli/actions/action_token/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
--rw-r--r--   0        0        0    35201 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12277 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
--rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/LICENSE
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/hatch.toml
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/pyproject.toml
--rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.54/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/action_generate/__init__.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/action_test/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/action_token/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
+-rw-r--r--   0        0        0    39032 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12277 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
+-rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/LICENSE
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/hatch.toml
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/pyproject.toml
+-rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cli/actions/action_generate/__init__.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/action_generate/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cli/actions/action_test/__init__.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/action_test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cli/actions/action_token/__init__.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/action_token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,15 +216,15 @@
   
   def general_boto_call_single(self, *args, **kwargs):
     data = self.general_boto_call_array(*args, **kwargs)
     if data is None or len(data) < 1:
       return None
     
     return data[0]
-
+  
   def general_boto_call_array(self, boto_call, boto_params, boto_key, boto_nextkey, retryCount = 10, verbose = False, boto_nextkey_param = None, error_codes_return = None, error_codes_continue = None, error_codes_raise = None, logger = None):
     return_data = []
 
     if boto_key is not None and self.get_common().helper_type().general().is_type(obj=boto_key, type_check= str):
       local_boto_key = boto_key
       boto_key = lambda item: item[local_boto_key] if item.get(local_boto_key) is not None else []
 
@@ -612,15 +612,15 @@
             if not item_key in regions:
               regions[item_key] = item
       return regions
     
     except Exception as err:
       self.get_common().get_logger().exception(msg=f"Could not pull regions dynamically: {err}", exc_info= err)
       return self.default_region_resources
-    
+  
   def get_accounts_regions_costexplorer(self, accounts, services, role= None):     
     if role is None:
       role = self.get_default_rolename()
     regions = { }
     
     for account in accounts:      
       regions[self.get_account_id(account)] = self.get_account_regions_costexplorer(
@@ -637,14 +637,114 @@
 
     return self._get_account_regions_costexplorer(
       account= account, 
       role= role,
       services= services
     )
   
+  def _get_regions_for_resource_configurationaggregator(self, account, role, configuration_accountId, configuration_aggregatorName, configuration_aggregatorRegion, configuration_aggregator_recourcetype):
+    
+    config_client = self.get_boto_client(
+      client= "config",
+      account= self.make_account(Id= configuration_accountId),
+      role= role,
+      region= configuration_aggregatorRegion)
+
+    retryCount = 10
+    currentAttempt = 0
+
+    filter = {}
+    filter["AccountId"] = self.get_account_id(account)    
+    filter["ResourceType"] =configuration_aggregator_recourcetype
+
+
+    while currentAttempt < retryCount:
+      currentAttempt+=1
+
+      try:
+        discovered_resources = config_client.get_aggregate_discovered_resource_counts(
+          ConfigurationAggregatorName = configuration_aggregatorName,
+          GroupByKey = "AWS_REGION",
+          Filters=filter
+          
+        )
+        break
+      except ClientError as err:
+        if currentAttempt > 2:
+          self.get_common().get_logger().exception(msg=f"_get_regions_for_resource: {err}", extra= {"exception": err})
+        discovered_resources = None
+        sleepTime = (2**currentAttempt)+randint(1,10)
+        if sleepTime > 30:
+          sleepTime = 30
+        time.sleep(sleepTime)
+
+    if discovered_resources is None:
+      return { }
+
+    regions = {self.get_account_id(account):[] }
+    for item in discovered_resources["GroupedResourceCounts"]:
+
+      if item["GroupName"] in regions[self.get_account_id(account)]:
+        continue
+
+      regions[self.get_account_id(account)].append(item["GroupName"])
+  
+    while "NextToken" in discovered_resources:
+      currentAttempt = 0
+      nextToken = discovered_resources["NextToken"]
+
+      while currentAttempt < retryCount:
+        currentAttempt+=1  
+        try:  
+          discovered_resources = config_client.get_aggregate_discovered_resource_counts(
+            ConfigurationAggregatorName = configuration_aggregatorName,
+            GroupByKey = "AWS_REGION",
+            Filters=filter,
+            NextToken= nextToken
+          )            
+          break
+            
+        except ClientError as err:
+          if currentAttempt > 2:
+            self.get_common().get_logger().exception(msg=f"_get_regions_for_resource - next loop: {err}", extra= {"exception": err})
+            print("_get_regions_for_resource - next loop: {}".format(err))
+          sleepTime = (2**currentAttempt)+randint(1,10)
+          if sleepTime > 30:
+            sleepTime = 30
+          time.sleep(sleepTime)        
+      
+      for item in discovered_resources["GroupedResourceCounts"]:
+        if item["GroupName"] in regions[self.get_account_id(account)]:
+          continue
+
+        regions[self.get_account_id(account)].append(item["GroupName"])
+
+
+    return regions
+  
+  def get_regions_account_configurationaggregator(self, accounts, role, configuration_accountId, configuration_aggregatorName, configuration_aggregatorRegion, configuration_aggregator_recourcetype):
+    regions = { }
+
+    for account in accounts:
+      if self.verbose:
+        if "accountName" in account:
+          print("Getting Regions for Account: {} ({})".format(self.get_account_name(account),self.get_account_id(account)))
+        else:
+          print("Getting Regions for Account: {}".format(self.get_account_id(account)))
+      for resource_type in configuration_aggregator_recourcetype:
+        tmpregions = self._get_regions_for_resource_configurationaggregator(account, role, configuration_accountId, configuration_aggregatorName, configuration_aggregatorRegion, resource_type)
+        for item in tmpregions:
+          if item in regions:
+            regions[item] = list(set(regions[item] + tmpregions[item]))    
+            continue
+
+          regions[item] = tmpregions[item]
+
+    return regions
+  
   def _get_accounts(self, refresh = False, include_suspended = False):
     
     if hasattr(self, "_account_list") and not refresh:
       return_list = "active" if not include_suspended else "all"
       if self._account_list is not None and len(self._account_list) > 0:
         if return_list in self._account_list:
           return self._account_list[return_list]
```

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/.gitignore` & `threemystic_cloud_client-0.1.55/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/LICENSE` & `threemystic_cloud_client-0.1.55/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/README.md` & `threemystic_cloud_client-0.1.55/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/hatch.toml` & `threemystic_cloud_client-0.1.55/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/pyproject.toml` & `threemystic_cloud_client-0.1.55/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.54/PKG-INFO` & `threemystic_cloud_client-0.1.55/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.54
+Version: 0.1.55
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

