# Comparing `tmp/threemystic_cloud_client-0.1.55.tar.gz` & `tmp/threemystic_cloud_client-0.1.56.tar.gz`

## Comparing `threemystic_cloud_client-0.1.55.tar` & `threemystic_cloud_client-0.1.56.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/action_generate/__init__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/action_test/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/action_token/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
--rw-r--r--   0        0        0    39032 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12277 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
--rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/LICENSE
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/hatch.toml
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/pyproject.toml
--rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.55/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cli/actions/action_generate/__init__.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cli/actions/action_test/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cli/actions/action_token/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
+-rw-r--r--   0        0        0    39185 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12277 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
+-rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/LICENSE
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/hatch.toml
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/pyproject.toml
+-rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.56/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/action_generate/__init__.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cli/actions/action_generate/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/action_test/__init__.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cli/actions/action_test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/action_token/__init__.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cli/actions/action_token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -570,15 +570,15 @@
         dt_format= "%Y-%m-%d"
       )),
       "End": (self.get_common().helper_type().datetime().datetime_as_string(
         dt= utc_now,
         dt_format= "%Y-%m-%d"
       ))
     }   
-    metrics = ["NET_UNBLENDED_COST"]
+    metrics = ["NETUNBLENDEDCOST"]
     group_by= [{"Type":"DIMENSION", "Key":"REGION"}]
 
     get_cost_usage_params = {
       "Granularity":granularity,
       "TimePeriod": time_period,
       "Metrics": metrics,
       "GroupBy": group_by
@@ -610,16 +610,19 @@
             if item_key == "noregion":
               continue
             if not item_key in regions:
               regions[item_key] = item
       return regions
     
     except Exception as err:
-      self.get_common().get_logger().exception(msg=f"Could not pull regions dynamically: {err}", exc_info= err)
-      return self.default_region_resources
+      print(err)
+      self.get_common().get_logger().exception(msg=f"Could not pull regions dynamically: {err}", extra= {"exception": err})
+      return {
+        self.get_common().helper_type().string().set_case(string_value= region, case= "lower"):region for region in self.default_region_resources
+      }
   
   def get_accounts_regions_costexplorer(self, accounts, services, role= None):     
     if role is None:
       role = self.get_default_rolename()
     regions = { }
     
     for account in accounts:
```

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.56/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/.gitignore` & `threemystic_cloud_client-0.1.56/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/LICENSE` & `threemystic_cloud_client-0.1.56/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/README.md` & `threemystic_cloud_client-0.1.56/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/hatch.toml` & `threemystic_cloud_client-0.1.56/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.55/pyproject.toml` & `threemystic_cloud_client-0.1.56/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
   "colorama; platform_system == 'Windows'",
   "threemystic-common >= 0.1.17",
   "polling2 >= 0.5.0",
   "typing-extensions >= 4.4.0",
   "pyopenssl >= 22.1.0",
   "PyJWT >= 2.7.0",
   "cryptography >= 41.0.1",
-  "boto3 >= 1.26.151",
-  "botocore >= 1.29.151",
+  "boto3 >= 1.28.15",
+  "botocore >= 1.31.16",
   "azure-common >= 1.1.28",
   "azure-cli >= 2.50.0",
   "azure-identity >= 1.13.0",
   "azure-mgmt-subscription >= 3.1.1",
   "azure-mgmt-managementgroups >= 1.0.0",
   "azure-mgmt-resourcegraph >= 8.0.0",
   "azure-mgmt-sql >= 3.0.1",
```

### Comparing `threemystic_cloud_client-0.1.55/PKG-INFO` & `threemystic_cloud_client-0.1.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.55
+Version: 0.1.56
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -20,16 +20,16 @@
 Requires-Dist: azure-cli>=2.50.0
 Requires-Dist: azure-common>=1.1.28
 Requires-Dist: azure-identity>=1.13.0
 Requires-Dist: azure-mgmt-managementgroups>=1.0.0
 Requires-Dist: azure-mgmt-resourcegraph>=8.0.0
 Requires-Dist: azure-mgmt-sql>=3.0.1
 Requires-Dist: azure-mgmt-subscription>=3.1.1
-Requires-Dist: boto3>=1.26.151
-Requires-Dist: botocore>=1.29.151
+Requires-Dist: boto3>=1.28.15
+Requires-Dist: botocore>=1.31.16
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: cryptography>=41.0.1
 Requires-Dist: polling2>=0.5.0
 Requires-Dist: pyjwt>=2.7.0
 Requires-Dist: pyopenssl>=22.1.0
 Requires-Dist: threemystic-common>=0.1.17
 Requires-Dist: typing-extensions>=4.4.0
```

