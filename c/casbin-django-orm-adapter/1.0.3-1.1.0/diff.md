# Comparing `tmp/casbin-django-orm-adapter-1.0.3.tar.gz` & `tmp/casbin-django-orm-adapter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin-django-orm-adapter-1.0.3.tar", last modified: Sat Jul 29 13:59:22 2023, max compression
+gzip compressed data, was "casbin-django-orm-adapter-1.1.0.tar", last modified: Mon Jul 31 16:26:22 2023, max compression
```

## Comparing `casbin-django-orm-adapter-1.0.3.tar` & `casbin-django-orm-adapter-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:59:22.587983 casbin-django-orm-adapter-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-29 13:59:22.587983 casbin-django-orm-adapter-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:59:22.587983 casbin-django-orm-adapter-1.0.3/casbin_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/enforcer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:59:22.587983 casbin-django-orm-adapter-1.0.3/casbin_adapter/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/casbin_adapter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:59:22.587983 casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-29 13:59:22.000000 casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-29 13:59:22.000000 casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 13:59:22.000000 casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 13:59:22.000000 casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 13:59:22.000000 casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-29 13:59:22.587983 casbin-django-orm-adapter-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:59:22.587983 casbin-django-orm-adapter-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-07-29 13:58:46.000000 casbin-django-orm-adapter-1.0.3/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:26:22.184070 casbin-django-orm-adapter-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-31 16:26:22.184070 casbin-django-orm-adapter-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:26:22.180070 casbin-django-orm-adapter-1.1.0/casbin_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/enforcer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:26:22.184070 casbin-django-orm-adapter-1.1.0/casbin_adapter/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/casbin_adapter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:26:22.184070 casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-31 16:26:22.000000 casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-31 16:26:22.000000 casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:26:22.000000 casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 16:26:22.000000 casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 16:26:22.000000 casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-31 16:26:22.184070 casbin-django-orm-adapter-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:26:22.184070 casbin-django-orm-adapter-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-07-31 16:25:51.000000 casbin-django-orm-adapter-1.1.0/tests/test_adapter.py
```

### Comparing `casbin-django-orm-adapter-1.0.3/LICENSE` & `casbin-django-orm-adapter-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.0.3/PKG-INFO` & `casbin-django-orm-adapter-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-django-orm-adapter
-Version: 1.0.3
+Version: 1.1.0
 Summary: Django's ORM adapter for PyCasbin
 Home-page: https://github.com/pycasbin/django-orm-adapter
 Author: Yang Luo
 Author-email: hsluoyz@qq.com
 License: Apache 2.0
 Keywords: casbin,adapter,storage-driver,django,orm,django-orm,access-control,authorization
 Classifier: Programming Language :: Python :: 3.7
@@ -86,24 +86,27 @@
 
 ## Configuration
 
 ### `CASBIN_MODEL`
 A string containing the file location of your casbin model.
 
 ### `CASBIN_ADAPTER`
-A string containing the adapter import path. Defaults to the django adapter shipped with this package: `casbin_adapter.adapter.Adapter`
+A string containing the adapter import path. Default to the django adapter shipped with this package: `casbin_adapter.adapter.Adapter`
 
 ### `CASBIN_ADAPTER_ARGS`
 A tuple of arguments to be passed into the constructor of the adapter specified
 in `CASBIN_ADAPTER`. Refer to adapters to see available arguments. 
 
 E.g. if you wish to use the file adapter 
 set the adapter to `casbin.persist.adapters.FileAdapter` and use
 `CASBIN_ADAPTER_ARGS = ('path/to/policy_file.csv',)`
 
+### `CASBIN_DB_ALIAS`
+The database the adapter uses. Default to "default".
+
 ### `CASBIN_WATCHER`
 Watcher instance to be set as the watcher on the enforcer instance.
 
 ### `CASBIN_ROLE_MANAGER`
 Role manager instance to be set as the role manager on the enforcer instance.
```

### Comparing `casbin-django-orm-adapter-1.0.3/README.md` & `casbin-django-orm-adapter-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -66,24 +66,27 @@
 
 ## Configuration
 
 ### `CASBIN_MODEL`
 A string containing the file location of your casbin model.
 
 ### `CASBIN_ADAPTER`
-A string containing the adapter import path. Defaults to the django adapter shipped with this package: `casbin_adapter.adapter.Adapter`
+A string containing the adapter import path. Default to the django adapter shipped with this package: `casbin_adapter.adapter.Adapter`
 
 ### `CASBIN_ADAPTER_ARGS`
 A tuple of arguments to be passed into the constructor of the adapter specified
 in `CASBIN_ADAPTER`. Refer to adapters to see available arguments. 
 
 E.g. if you wish to use the file adapter 
 set the adapter to `casbin.persist.adapters.FileAdapter` and use
 `CASBIN_ADAPTER_ARGS = ('path/to/policy_file.csv',)`
 
+### `CASBIN_DB_ALIAS`
+The database the adapter uses. Default to "default".
+
 ### `CASBIN_WATCHER`
 Watcher instance to be set as the watcher on the enforcer instance.
 
 ### `CASBIN_ROLE_MANAGER`
 Role manager instance to be set as the role manager on the enforcer instance.
```

### Comparing `casbin-django-orm-adapter-1.0.3/casbin_adapter/adapter.py` & `casbin-django-orm-adapter-1.1.0/casbin_adapter/adapter.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Adapter(persist.Adapter):
     """the interface for Casbin adapters."""
 
+    def __init__(self, db_alias="default"):
+        self.db_alias = db_alias
+
     def load_policy(self, model):
         """loads all policy rules from the storage."""
         try:
-            lines = CasbinRule.objects.all()
+            lines = CasbinRule.objects.using(self.db_alias).all()
 
             for line in lines:
                 persist.load_policy_line(str(line), model)
         except (OperationalError, ProgrammingError) as error:
             logger.warning("Could not load policy from database: {}".format(error))
 
     def _create_policy_line(self, ptype, rule):
@@ -37,45 +40,45 @@
             line.v5 = rule[5]
         return line
 
     def save_policy(self, model):
         """saves all policy rules to the storage."""
         # See https://casbin.org/docs/en/adapters#autosave
         # for why this is deleting all rules
-        CasbinRule.objects.all().delete()
+        CasbinRule.objects.using(self.db_alias).all().delete()
 
         lines = []
         for sec in ["p", "g"]:
             if sec not in model.model.keys():
                 continue
             for ptype, ast in model.model[sec].items():
                 for rule in ast.policy:
                     lines.append(self._create_policy_line(ptype, rule))
-        CasbinRule.objects.bulk_create(lines)
+        CasbinRule.objects.using(self.db_alias).bulk_create(lines)
         return True
 
     def add_policy(self, sec, ptype, rule):
         """adds a policy rule to the storage."""
         line = self._create_policy_line(ptype, rule)
         line.save()
 
     def remove_policy(self, sec, ptype, rule):
         """removes a policy rule from the storage."""
         query_params = {"ptype": ptype}
         for i, v in enumerate(rule):
             query_params["v{}".format(i)] = v
-        rows_deleted, _ = CasbinRule.objects.filter(**query_params).delete()
+        rows_deleted, _ = CasbinRule.objects.using(self.db_alias).filter(**query_params).delete()
         return True if rows_deleted > 0 else False
 
     def remove_filtered_policy(self, sec, ptype, field_index, *field_values):
         """removes policy rules that match the filter from the storage.
         This is part of the Auto-Save feature.
         """
         query_params = {"ptype": ptype}
         if not (0 <= field_index <= 5):
             return False
         if not (1 <= field_index + len(field_values) <= 6):
             return False
         for i, v in enumerate(field_values):
             query_params["v{}".format(i + field_index)] = v
-        rows_deleted, _ = CasbinRule.objects.filter(**query_params).delete()
+        rows_deleted, _ = CasbinRule.objects.using(self.db_alias).filter(**query_params).delete()
         return True if rows_deleted > 0 else False
```

### Comparing `casbin-django-orm-adapter-1.0.3/casbin_adapter/migrations/0001_initial.py` & `casbin-django-orm-adapter-1.1.0/casbin_adapter/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.0.3/casbin_adapter/models.py` & `casbin-django-orm-adapter-1.1.0/casbin_adapter/models.py`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/PKG-INFO` & `casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-django-orm-adapter
-Version: 1.0.3
+Version: 1.1.0
 Summary: Django's ORM adapter for PyCasbin
 Home-page: https://github.com/pycasbin/django-orm-adapter
 Author: Yang Luo
 Author-email: hsluoyz@qq.com
 License: Apache 2.0
 Keywords: casbin,adapter,storage-driver,django,orm,django-orm,access-control,authorization
 Classifier: Programming Language :: Python :: 3.7
@@ -86,24 +86,27 @@
 
 ## Configuration
 
 ### `CASBIN_MODEL`
 A string containing the file location of your casbin model.
 
 ### `CASBIN_ADAPTER`
-A string containing the adapter import path. Defaults to the django adapter shipped with this package: `casbin_adapter.adapter.Adapter`
+A string containing the adapter import path. Default to the django adapter shipped with this package: `casbin_adapter.adapter.Adapter`
 
 ### `CASBIN_ADAPTER_ARGS`
 A tuple of arguments to be passed into the constructor of the adapter specified
 in `CASBIN_ADAPTER`. Refer to adapters to see available arguments. 
 
 E.g. if you wish to use the file adapter 
 set the adapter to `casbin.persist.adapters.FileAdapter` and use
 `CASBIN_ADAPTER_ARGS = ('path/to/policy_file.csv',)`
 
+### `CASBIN_DB_ALIAS`
+The database the adapter uses. Default to "default".
+
 ### `CASBIN_WATCHER`
 Watcher instance to be set as the watcher on the enforcer instance.
 
 ### `CASBIN_ROLE_MANAGER`
 Role manager instance to be set as the role manager on the enforcer instance.
```

### Comparing `casbin-django-orm-adapter-1.0.3/casbin_django_orm_adapter.egg-info/SOURCES.txt` & `casbin-django-orm-adapter-1.1.0/casbin_django_orm_adapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.0.3/setup.py` & `casbin-django-orm-adapter-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `casbin-django-orm-adapter-1.0.3/tests/test_adapter.py` & `casbin-django-orm-adapter-1.1.0/tests/test_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import casbin
 import simpleeval
-from unittest import TestCase
 
 from django.test import TestCase
 from casbin_adapter.models import CasbinRule
 from casbin_adapter.adapter import Adapter
 
 
 def get_fixture(path):
```

