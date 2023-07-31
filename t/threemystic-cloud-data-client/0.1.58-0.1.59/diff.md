# Comparing `tmp/threemystic_cloud_data_client-0.1.58.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.59.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.58.tar` & `threemystic_cloud_data_client-0.1.59.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0    17841 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py
--rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
--rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py
--rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    23458 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
--rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    13572 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/hatch.toml
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/pyproject.toml
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.58/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0    17266 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py
+-rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
+-rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py
+-rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    23458 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    13572 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/hatch.toml
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/pyproject.toml
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.59/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/budget.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,14 @@
     super().__init__(
       data_action="budget",
       logger_name= "cloud_data_client_aws_client_action_budget",
       *args, **kwargs)
   
   async def _process_account_data_region(self, account, region, resource_groups, loop, *args, **kwargs):
     pass
-  
-  def __get_costdata_total_key(self, forecast_metric, *args, **kwargs):
-    if self.get_common().helper_type().string().set_case(string_value= forecast_metric, case= "upper") == "NET_UNBLENDED_COST":
-      return "NetUnblendedCost"
 
   def __init_costdata_month(self, data_dt, *args, **kwargs):
     return {
       "currency": self.get_common().helper_type().string().set_case(self.get_cloud_data_client().get_default_currency(), case= "upper"),
       "month": data_dt.month,
       "year": data_dt.year,
       "totals":{
@@ -62,15 +58,15 @@
         "total":{},
         "forcast_total":{},
         "origional_currency_total":{},
         "origional_currency_forcast_total":{},
       }
     }
   
-  async def __process_get_cost_data_process_forcast(self, year_data, client, account, start_date, end_date, fiscal_start, fiscal_end, forecast_metrics = ["NET_UNBLENDED_COST"], *args, **kwargs):
+  async def __process_get_cost_data_process_forcast(self, year_data, client, account, start_date, end_date, fiscal_start, fiscal_end, forecast_metrics, *args, **kwargs):
     
     results_by_time_forcast = self.get_cloud_client().general_boto_call_array(
       boto_call=lambda: client.get_cost_and_usage(
         TimePeriod={
           'Start': start_date.strftime("%Y-%m-%d"),
           'End': end_date.strftime("%Y-%m-%d"),
         },
@@ -124,15 +120,15 @@
         year_data[forecast_metric][by_month_key]["days"][day_key][f'origional_currency_{total_key}'] += Decimal(raw_row_data_cost)
         year_data[forecast_metric][by_month_key]["days"][day_key][f'{total_key}'] += Decimal(row_data_cost)
         year_data[forecast_metric][by_month_key]["totals"][f'{total_key}'] += Decimal(row_data_cost)
         if data_dt >= fiscal_start and data_dt <= fiscal_end:
           year_data[forecast_metric][by_month_key]["totals"][f'fiscal_{total_key}'] += Decimal(row_data_cost)
 
 
-  async def __process_get_cost_data_process_year_data(self, year_data, client, account, start_date, end_date, fiscal_start, fiscal_end, forecast_metrics = ["NET_UNBLENDED_COST"], *args, **kwargs):
+  async def __process_get_cost_data_process_year_data(self, year_data, client, account, start_date, end_date, fiscal_start, fiscal_end, forecast_metrics, *args, **kwargs):
 
     results_by_time = self.get_cloud_client().general_boto_call_array(
       boto_call=lambda: client.get_cost_and_usage(
         TimePeriod={
           'Start': start_date.strftime("%Y-%m-%d"),
           'End': end_date.strftime("%Y-%m-%d"),
         },
@@ -165,18 +161,18 @@
         by_month_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m", dt= data_dt)
 
         day_key = self.get_common().helper_type().datetime().datetime_as_string(dt_format= "%Y%m%d", dt= data_dt)
         if year_data[forecast_metric].get(by_month_key) is None:
           year_data[forecast_metric][by_month_key] = self.__init_costdata_month(data_dt= data_dt)
         
         if year_data[forecast_metric][by_month_key]["days"].get(day_key) is None:
-          year_data[forecast_metric][by_month_key]["days"][day_key] = self.__init_costdata_month_day(data_dt= data_dt, currency= cost_data["Total"][self.__get_costdata_total_key(forecast_metric= forecast_metric)]["Unit"])
+          year_data[forecast_metric][by_month_key]["days"][day_key] = self.__init_costdata_month_day(data_dt= data_dt, currency= cost_data["Total"][forecast_metric]["Unit"])
         
-        raw_row_data_cost = (cost_data["Total"][self.__get_costdata_total_key(forecast_metric= forecast_metric)]["Amount"])
-        row_data_cost = (cost_data["Total"][self.__get_costdata_total_key(forecast_metric= forecast_metric)]["Amount"])
+        raw_row_data_cost = (cost_data["Total"][forecast_metric]["Amount"])
+        row_data_cost = (cost_data["Total"][forecast_metric]["Amount"])
         
         if year_data[forecast_metric][by_month_key]["days"][day_key]["currency"] != year_data[forecast_metric][by_month_key]["days"][day_key]["origional_currency"]:
           row_data_cost = self.get_common().helper_currency().convert(
             ammount= row_data_cost,
             currency_from= year_data[forecast_metric][by_month_key]["days"][day_key]["origional_currency"],
             currency_to= year_data[forecast_metric][by_month_key]["days"][day_key]["currency"],
             conversion_date= self.get_common().helper_type().datetime().yesterday(dt=self.get_common().helper_type().datetime().datetime_from_string(
@@ -191,21 +187,21 @@
         year_data[forecast_metric][by_month_key]["days"][day_key][f'origional_currency_{total_key}'] += Decimal(raw_row_data_cost)
         year_data[forecast_metric][by_month_key]["days"][day_key][f'{total_key}'] += Decimal(row_data_cost)
         year_data[forecast_metric][by_month_key]["totals"][f'{total_key}'] += Decimal(row_data_cost)
         if data_dt >= fiscal_start and data_dt <= fiscal_end:
           year_data[forecast_metric][by_month_key]["totals"][f'fiscal_{total_key}'] += Decimal(row_data_cost)
 
         for cost_data_group in cost_data["Groups"]:
-          raw_row_data_cost_group = cost_data_group["Metrics"][self.__get_costdata_total_key(forecast_metric= forecast_metric)]["Amount"]
+          raw_row_data_cost_group = cost_data_group["Metrics"][forecast_metric]["Amount"]
           row_data_cost_group = raw_row_data_cost_group
           
-          if year_data[forecast_metric][by_month_key]["days"][day_key]["currency"] != cost_data_group["Metrics"][self.__get_costdata_total_key(forecast_metric= forecast_metric)]["Unit"]:
+          if year_data[forecast_metric][by_month_key]["days"][day_key]["currency"] != cost_data_group["Metrics"][forecast_metric]["Unit"]:
             row_data_cost_group = self.get_common().helper_currency().convert(
               ammount= row_data_cost_group,
-              currency_from= cost_data_group["Metrics"][self.__get_costdata_total_key(forecast_metric= forecast_metric)]["Unit"],
+              currency_from= cost_data_group["Metrics"][forecast_metric]["Unit"],
               currency_to= year_data[forecast_metric][by_month_key]["days"][day_key]["currency"],
               conversion_date= self.get_common().helper_type().datetime().yesterday(dt=self.get_common().helper_type().datetime().datetime_from_string(
                 dt_string= self.get_common().helper_type().datetime().datetime_as_string(
                   dt= data_dt,
                   dt_format= "%Y%m01"
                 ),
                 dt_format= "%Y%m%d"
@@ -245,15 +241,15 @@
                  + self.get_common().helper_type().datetime().time_delta(months= -1, dt= fiscal_year_start_date))
     
     forecast_end = (fiscal_year_end
                  + self.get_common().helper_type().datetime().time_delta(months= 3, dt= fiscal_year_end))
     
 
     year_data = {}
-    forcast_metric = "NET_UNBLENDED_COST"
+    forcast_metric = "NetUnblendedCost"
     await self.__process_get_cost_data_process_year_data(
       year_data= year_data,
       client= client,
       account= account,
       start_date= start_date,
       end_date= self.get_data_start() if forecast_end > self.get_data_start() else forecast_end,
       fiscal_start= fiscal_year_start_date,
```

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/dns.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/memorydb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py` & `threemystic_cloud_data_client-0.1.59/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/.gitignore` & `threemystic_cloud_data_client-0.1.59/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/LICENSE` & `threemystic_cloud_data_client-0.1.59/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/README.md` & `threemystic_cloud_data_client-0.1.59/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/hatch.toml` & `threemystic_cloud_data_client-0.1.59/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.58/pyproject.toml` & `threemystic_cloud_data_client-0.1.59/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
   "threemystic-common >= 0.1.17",
-  "threemystic-cloud-client >= 0.1.55",
+  "threemystic-cloud-client >= 0.1.56",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
   "azure-mgmt-compute >= 29",
   "azure-mgmt-cosmosdb >= 9",
   "azure-mgmt-costmanagement >= 4",
   "azure-mgmt-dns >= 8",
```

### Comparing `threemystic_cloud_data_client-0.1.58/PKG-INFO` & `threemystic_cloud_data_client-0.1.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.58
+Version: 0.1.59
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,15 @@
 Requires-Dist: azure-mgmt-redis>=14
 Requires-Dist: azure-mgmt-resourcegraph>=8
 Requires-Dist: azure-mgmt-sql>=3
 Requires-Dist: azure-mgmt-sqlvirtualmachine>=0.6
 Requires-Dist: azure-mgmt-subscription>=3
 Requires-Dist: azure-mgmt-synapse>=2
 Requires-Dist: colorama; platform_system == 'Windows'
-Requires-Dist: threemystic-cloud-client>=0.1.55
+Requires-Dist: threemystic-cloud-client>=0.1.56
 Requires-Dist: threemystic-common>=0.1.17
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_data_client
 A set of scripts to help uniformly pull data from the cloud providers for various resources.
```

