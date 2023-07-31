# Comparing `tmp/octodns-azure-0.0.4.tar.gz` & `tmp/octodns-azure-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns-azure-0.0.4.tar", last modified: Wed Nov 30 20:29:44 2022, max compression
+gzip compressed data, was "octodns-azure-0.0.5.tar", last modified: Mon Jul 31 18:06:03 2023, max compression
```

## Comparing `octodns-azure-0.0.4.tar` & `octodns-azure-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2022-11-30 20:29:44.878930 octodns-azure-0.0.4/
--rw-r--r--   0 ross       (501) staff       (20)     5259 2022-11-30 20:29:44.878556 octodns-azure-0.0.4/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)     4919 2022-10-26 15:19:51.000000 octodns-azure-0.0.4/README.md
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2022-11-30 20:29:44.874427 octodns-azure-0.0.4/octodns_azure/
--rw-r--r--   0 ross       (501) staff       (20)    62705 2022-11-30 20:29:30.000000 octodns-azure-0.0.4/octodns_azure/__init__.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2022-11-30 20:29:44.876489 octodns-azure-0.0.4/octodns_azure.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)     5259 2022-11-30 20:29:44.000000 octodns-azure-0.0.4/octodns_azure.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      244 2022-11-30 20:29:44.000000 octodns-azure-0.0.4/octodns_azure.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2022-11-30 20:29:44.000000 octodns-azure-0.0.4/octodns_azure.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)      345 2022-11-30 20:29:44.000000 octodns-azure-0.0.4/octodns_azure.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       18 2022-11-30 20:29:44.000000 octodns-azure-0.0.4/octodns_azure.egg-info/top_level.txt
--rw-r--r--   0 ross       (501) staff       (20)       38 2022-11-30 20:29:44.879035 octodns-azure-0.0.4/setup.cfg
--rw-r--r--   0 ross       (501) staff       (20)     1885 2022-10-26 15:19:51.000000 octodns-azure-0.0.4/setup.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2022-11-30 20:29:44.876779 octodns-azure-0.0.4/tmp/
--rw-r--r--   0 ross       (501) staff       (20)    59421 2022-02-09 18:34:41.000000 octodns-azure-0.0.4/tmp/__init__.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-07-31 18:06:03.674162 octodns-azure-0.0.5/
+-rw-r--r--   0 neo       (1000) neo       (1000)     5644 2023-07-31 18:06:03.674162 octodns-azure-0.0.5/PKG-INFO
+-rw-r--r--   0 neo       (1000) neo       (1000)     5304 2023-07-26 09:39:47.000000 octodns-azure-0.0.5/README.md
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-07-31 18:06:03.670828 octodns-azure-0.0.5/octodns_azure/
+-rw-r--r--   0 neo       (1000) neo       (1000)    69069 2023-07-31 17:58:24.000000 octodns-azure-0.0.5/octodns_azure/__init__.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-07-31 18:06:03.670828 octodns-azure-0.0.5/octodns_azure.egg-info/
+-rw-r--r--   0 neo       (1000) neo       (1000)     5644 2023-07-31 18:06:03.000000 octodns-azure-0.0.5/octodns_azure.egg-info/PKG-INFO
+-rw-r--r--   0 neo       (1000) neo       (1000)      272 2023-07-31 18:06:03.000000 octodns-azure-0.0.5/octodns_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)        1 2023-07-31 18:06:03.000000 octodns-azure-0.0.5/octodns_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)      425 2023-07-31 18:06:03.000000 octodns-azure-0.0.5/octodns_azure.egg-info/requires.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       14 2023-07-31 18:06:03.000000 octodns-azure-0.0.5/octodns_azure.egg-info/top_level.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)      306 2023-04-17 20:24:34.000000 octodns-azure-0.0.5/pyproject.toml
+-rw-r--r--   0 neo       (1000) neo       (1000)       38 2023-07-31 18:06:03.674162 octodns-azure-0.0.5/setup.cfg
+-rw-r--r--   0 neo       (1000) neo       (1000)     2323 2023-07-31 17:58:24.000000 octodns-azure-0.0.5/setup.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-07-31 18:06:03.670828 octodns-azure-0.0.5/tests/
+-rw-r--r--   0 neo       (1000) neo       (1000)   141822 2023-07-26 09:39:47.000000 octodns-azure-0.0.5/tests/test_provider_azure.py
```

### Comparing `octodns-azure-0.0.4/PKG-INFO` & `octodns-azure-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: octodns-azure
-Version: 0.0.4
+Version: 0.0.5
 Summary:  Azure DNS & TrafficManager provider for octoDNS
 Home-page: https://github.com/octodns/octodns-azure
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 
 ## Azure DNS & TrafficManager provider for octoDNS
 
 An [octoDNS](https://github.com/octodns/octodns/) provider that targets [Azure](https://azure.microsoft.com/en-us/services/dns/#overview).
@@ -66,18 +66,24 @@
     # All are required to authenticate.
     # Azure RetryPolicy Settings all of them are optional.
     # https://azuresdkdocs.blob.core.windows.net/$web/python/azure-core/1.9.0/azure.core.pipeline.policies.html?highlight=retrypolicy#azure.core.pipeline.policies.RetryPolicy
     # Total_retries default 10
     #client_total_retries: 10
     # status_retries default 3
     #client_status_retries: 3
+    # The maximum number of record sets to return per page.
+    # https://learn.microsoft.com/en-us/rest/api/dns/record-sets/list-by-dns-zone
+    # Top default 100
+    #top: 100
 ```
 
 The first four variables above can be hidden in environment variables and octoDNS will automatically search for them in the shell. It is possible to also hard-code into the config file: eg, resource_group.
 
+For management of DNS zones on [Azure Private DNS](https://learn.microsoft.com/en-us/azure/dns/private-dns-overview), use `class: octodns_azure.AzurePrivateProvider`. Note that this provider does not support dynamic records or root NS records.
+
 ### Support Information
 
 #### Records
 
 AzureProvider supports A, AAAA, CAA, CNAME, MX, NS, PTR, SRV, and TXT
 
 #### Root NS Records
@@ -101,15 +107,15 @@
 | num_failures | This value specifies how many failures a Traffic Manager probing agent tolerates before marking that endpoint as unhealthy. Its value can range between 0 and 9. A value of 0 means a single monitoring failure can cause that endpoint to be marked as unhealthy. If no value is specified, it uses the default value of 3. | 3 |
 
 ```
 ---
   octodns:
     azuredns:
       healthcheck:
-        interval_in_seconds: 10
-        timeout_in_seconds: 7
-        tolerated_number_of_failures: 4
+        interval: 10
+        timeout: 7
+        num_failures: 4
 ```
 
 ### Development
 
 See the [/script/](/script/) directory for some tools to help with the development process. They generally follow the [Script to rule them all](https://github.com/github/scripts-to-rule-them-all) pattern. Most useful is `./script/bootstrap` which will create a venv and install both the runtime and development related requirements. It will also hook up a pre-commit hook that covers most of what's run by CI.
```

### Comparing `octodns-azure-0.0.4/README.md` & `octodns-azure-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -53,18 +53,24 @@
     # All are required to authenticate.
     # Azure RetryPolicy Settings all of them are optional.
     # https://azuresdkdocs.blob.core.windows.net/$web/python/azure-core/1.9.0/azure.core.pipeline.policies.html?highlight=retrypolicy#azure.core.pipeline.policies.RetryPolicy
     # Total_retries default 10
     #client_total_retries: 10
     # status_retries default 3
     #client_status_retries: 3
+    # The maximum number of record sets to return per page.
+    # https://learn.microsoft.com/en-us/rest/api/dns/record-sets/list-by-dns-zone
+    # Top default 100
+    #top: 100
 ```
 
 The first four variables above can be hidden in environment variables and octoDNS will automatically search for them in the shell. It is possible to also hard-code into the config file: eg, resource_group.
 
+For management of DNS zones on [Azure Private DNS](https://learn.microsoft.com/en-us/azure/dns/private-dns-overview), use `class: octodns_azure.AzurePrivateProvider`. Note that this provider does not support dynamic records or root NS records.
+
 ### Support Information
 
 #### Records
 
 AzureProvider supports A, AAAA, CAA, CNAME, MX, NS, PTR, SRV, and TXT
 
 #### Root NS Records
@@ -88,15 +94,15 @@
 | num_failures | This value specifies how many failures a Traffic Manager probing agent tolerates before marking that endpoint as unhealthy. Its value can range between 0 and 9. A value of 0 means a single monitoring failure can cause that endpoint to be marked as unhealthy. If no value is specified, it uses the default value of 3. | 3 |
 
 ```
 ---
   octodns:
     azuredns:
       healthcheck:
-        interval_in_seconds: 10
-        timeout_in_seconds: 7
-        tolerated_number_of_failures: 4
+        interval: 10
+        timeout: 7
+        num_failures: 4
 ```
 
 ### Development
 
 See the [/script/](/script/) directory for some tools to help with the development process. They generally follow the [Script to rule them all](https://github.com/github/scripts-to-rule-them-all) pattern. Most useful is `./script/bootstrap` which will create a venv and install both the runtime and development related requirements. It will also hook up a pre-commit hook that covers most of what's run by CI.
```

### Comparing `octodns-azure-0.0.4/octodns_azure/__init__.py` & `octodns-azure-0.0.5/octodns_azure/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,44 +2,47 @@
 #
 #
 
 from collections import defaultdict
 from functools import reduce
 from logging import getLogger
 
+from azure.core.pipeline.policies import RetryPolicy
 from azure.identity import ClientSecretCredential
 from azure.mgmt.dns import DnsManagementClient
-from azure.mgmt.trafficmanager import TrafficManagerManagementClient
-from azure.core.pipeline.policies import RetryPolicy
-
 from azure.mgmt.dns.models import (
-    ARecord,
     AaaaRecord,
+    ARecord,
     CaaRecord,
     CnameRecord,
     MxRecord,
-    SrvRecord,
     NsRecord,
     PtrRecord,
+    SrvRecord,
     TxtRecord,
     Zone,
 )
+from azure.mgmt.privatedns import PrivateDnsManagementClient
+from azure.mgmt.privatedns.models import PrivateZone
+from azure.mgmt.trafficmanager import TrafficManagerManagementClient
 from azure.mgmt.trafficmanager.models import (
-    Profile,
+    AlwaysServe,
     DnsConfig,
-    MonitorConfig,
     Endpoint,
+    EndpointStatus,
+    MonitorConfig,
     MonitorConfigCustomHeadersItem,
+    Profile,
 )
 
-from octodns.record import Record, Update, GeoCodes
 from octodns.provider import ProviderException
 from octodns.provider.base import BaseProvider
+from octodns.record import GeoCodes, Record, Update
 
-__VERSION__ = '0.0.4'
+__VERSION__ = '0.0.5'
 
 
 class AzureException(ProviderException):
     pass
 
 
 def escape_semicolon(s):
@@ -241,15 +244,14 @@
         try:
             values = data['values']
         except KeyError:
             values = [data['value']]
         return {key_name: [azure_class(ptrdname=v) for v in values]}
 
     def _params_for_TXT(self, data, key_name, azure_class):
-
         params = []
         try:  # API for TxtRecord has list of str, even for singleton
             values = [v for v in azure_chunked_values(data['values'])]
         except KeyError:
             values = [azure_chunked_value(data['value'])]
 
         for v in values:
@@ -369,31 +371,19 @@
         ]
     return monitor
 
 
 def _check_valid_dynamic(record):
     typ = record._type
     if typ in ['A', 'AAAA']:
-        defaults = set(record.values)
-        if len(defaults) > 1:
-            pools = record.dynamic.pools
-            vals = set(
-                v['value']
-                for _, pool in pools.items()
-                for v in pool._data()['values']
-            )
-            if defaults != vals:
-                # we don't yet support multi-value defaults, specifying all
-                # pool values allows for Traffic Manager profile optimization
-                raise AzureException(
-                    f'{record.fqdn} {record._type}: Values '
-                    'of A/AAAA dynamic records must either '
-                    'have a single value or contain all '
-                    'values from all pools'
-                )
+        if len(record.values) > 1:
+            # we don't yet support multi-value defaults
+            raise AzureException(
+                f'{record.fqdn} {record._type}: Dynamic records do not support multiple top-level values'
+            )
     elif typ != 'CNAME':
         # dynamic records of unsupported type
         raise AzureException(
             f'{record.fqdn}: Dynamic records in Azure must '
             'be of type A/AAAA/CNAME'
         )
 
@@ -455,22 +445,30 @@
         have_endpoints = sorted(have.endpoints, key=lambda e: e.target)
         desired_endpoints = sorted(desired.endpoints, key=lambda e: e.target)
     else:
         have_endpoints = have.endpoints
         desired_endpoints = desired.endpoints
     endpoints = zip(have_endpoints, desired_endpoints)
     for have_endpoint, desired_endpoint in endpoints:
-        have_status = have_endpoint.endpoint_status or 'Enabled'
-        desired_status = desired_endpoint.endpoint_status or 'Enabled'
+        have_status = have_endpoint.endpoint_status or EndpointStatus.ENABLED
+        desired_status = (
+            desired_endpoint.endpoint_status or EndpointStatus.ENABLED
+        )
+
+        have_always_serve = have_endpoint.always_serve or AlwaysServe.DISABLED
+        desired_always_serve = (
+            desired_endpoint.always_serve or AlwaysServe.DISABLED
+        )
 
         # compare basic attributes
         if (
             have_endpoint.name != desired_endpoint.name
             or have_endpoint.type != desired_endpoint.type
             or have_status != desired_status
+            or have_always_serve != desired_always_serve
         ):
             return false(have_endpoint, desired_endpoint, have.name)
 
         # compare geos
         if method == 'Geographic':
             have_geos = sorted(have_endpoint.geo_mapping)
             desired_geos = sorted(desired_endpoint.geo_mapping)
@@ -505,71 +503,44 @@
         else:
             # unexpected, give up
             return False
 
     return True
 
 
-class AzureProvider(BaseProvider):
-    '''
-    Azure DNS Provider
+def _endpoint_flags_to_value_status(endpoint_status, always_serve):
+    """Convert between azure endpoint's endpoint_status and always_serve flags and octo's pool status flag"""
+    if endpoint_status is None:
+        endpoint_status = EndpointStatus.ENABLED
+    if always_serve is None:
+        always_serve = AlwaysServe.DISABLED
+
+    if endpoint_status == EndpointStatus.DISABLED:
+        # It doesn't matter what always_serve is if endpoint is disabled
+        return 'down'
+    elif always_serve == AlwaysServe.ENABLED:
+        return 'up'
+    else:
+        return 'obey'
 
-    azuredns.py:
-        class: octodns.provider.azuredns.AzureProvider
-        # Current support of authentication of access to Azure services only
-        # includes using a Service Principal:
-        # https://docs.microsoft.com/en-us/azure/azure-resource-manager/
-        #                        resource-group-create-service-principal-portal
-        # The Azure Active Directory Application ID (aka client ID):
-        client_id:
-        # Authentication Key Value: (note this should be secret)
-        key:
-        # Directory ID (aka tenant ID):
-        directory_id:
-        # Subscription ID:
-        sub_id:
-        # Resource Group name:
-        resource_group:
-        # All are required to authenticate.
 
-        Example config file with variables:
-            "
-            ---
-            providers:
-              config:
-                class: octodns.provider.yaml.YamlProvider
-                directory: ./config (example path to directory of zone files)
-              azuredns:
-                class: octodns.provider.azuredns.AzureProvider
-                client_id: env/AZURE_APPLICATION_ID
-                key: env/AZURE_AUTHENTICATION_KEY
-                directory_id: env/AZURE_DIRECTORY_ID
-                sub_id: env/AZURE_SUBSCRIPTION_ID
-                resource_group: 'TestResource1'
-
-            zones:
-              example.com.:
-                sources:
-                  - config
-                targets:
-                  - azuredns
-            "
-        The first four variables above can be hidden in environment variables
-        and octoDNS will automatically search for them in the shell. It is
-        possible to also hard-code into the config file: eg, resource_group.
+def _value_status_to_endpoint_flags(value_status):
+    """Convert between octo's pool status flag and azure endpoint's endpoint_status and always_serve flags"""
+    status_map = {
+        'down': (EndpointStatus.DISABLED, AlwaysServe.DISABLED),
+        'up': (EndpointStatus.ENABLED, AlwaysServe.ENABLED),
+        'obey': (EndpointStatus.ENABLED, AlwaysServe.DISABLED),
+    }
+    return status_map[value_status]
 
-        Please read https://github.com/octodns/octodns/pull/706 for an overview
-        of how dynamic records are designed and caveats of using them.
-    '''
 
+class AzureBaseProvider(BaseProvider):
     SUPPORTS_GEO = False
-    SUPPORTS_DYNAMIC = True
     SUPPORTS_POOL_VALUE_STATUS = True
     SUPPORTS_MULTIVALUE_PTR = True
-    SUPPORTS_ROOT_NS = True
     SUPPORTS = set(
         ('A', 'AAAA', 'CAA', 'CNAME', 'MX', 'NS', 'PTR', 'SRV', 'TXT')
     )
 
     def __init__(
         self,
         id,
@@ -578,44 +549,46 @@
         directory_id,
         sub_id,
         resource_group,
         client_total_retries=10,
         client_status_retries=3,
         authority="https://login.microsoftonline.com",
         base_url="https://management.azure.com",
+        top=100,
         *args,
         **kwargs,
     ):
-        self.log = getLogger(f'AzureProvider[{id}]')
+        self.log = getLogger(f'{self.__class__.__name__}[{id}]')
         self.log.debug(
             '__init__: id=%s, client_id=%s, '
             'key=***, directory_id:%s, authority:%s, '
             'base_url:%s, client_total_retries:%d, '
-            'client_status_retries:%d',
+            'client_status_retries:%d, top:%d',
             id,
             client_id,
             directory_id,
             authority,
             base_url,
             client_total_retries,
             client_status_retries,
+            top,
         )
         super().__init__(id, *args, **kwargs)
 
         # Store necessary initialization params
         self._authority = authority
         self._base_url = base_url
         self._client_client_id = client_id
         self._client_key = key
         self._client_directory_id = directory_id
         self._client_subscription_id = sub_id
         self.__client_credential = None
 
-        self.__dns_client = None
-        self.__tm_client = None
+        self._dns_client = None
+        self._dns_client_top = top
 
         self._resource_group = resource_group
         self._traffic_managers = dict()
 
         self.__azure_zones = None
         self._required_root_ns_values = {}
 
@@ -639,40 +612,19 @@
                 tenant_id=self._client_directory_id,
                 authority=self._authority,
                 logger=logger,
             )
         return self.__client_credential
 
     @property
-    def _dns_client(self):
-        if self.__dns_client is None:
-            self.__dns_client = DnsManagementClient(
-                credential=self._client_credential,
-                subscription_id=self._client_subscription_id,
-                retry_policy=self._dns_client_retry_policy,
-                base_url=self._base_url,
-            )
-        return self.__dns_client
-
-    @property
-    def _tm_client(self):
-        if self.__tm_client is None:
-            self.__tm_client = TrafficManagerManagementClient(
-                credential=self._client_credential,
-                subscription_id=self._client_subscription_id,
-                base_url=self._base_url,
-            )
-        return self.__tm_client
-
-    @property
     def _azure_zones(self):
         if self.__azure_zones is None:
             self.log.debug('_azure_zones: loading')
             zones = set()
-            list_zones = self._dns_client.zones.list_by_resource_group
+            list_zones = self._dns_client_zones().list_by_resource_group
             for zone in list_zones(self._resource_group):
                 zones.add(zone.name.rstrip('.'))
             self.__azure_zones = zones
 
         return self.__azure_zones
 
     def _check_zone(self, name, create=False):
@@ -691,69 +643,26 @@
         self.log.debug('_check_zone: name=%s create=%s', name, create)
         # Check if the zone already exists in our set
         if name in self._azure_zones:
             return name
         # If not, and its time to create, lets do it.
         if create:
             self.log.debug('_check_zone:no matching zone; creating %s', name)
-            create_zone = self._dns_client.zones.create_or_update
-            zone = create_zone(
-                self._resource_group, name, Zone(location='global')
-            )
+            zone = self._create_zone(name)
             self._azure_zones.add(name)
 
             # we create the zone so we should now be able to get its root ns
             # records
             self._required_root_ns_values[name] = set(zone.name_servers)
 
             return name
         else:
             # Else return nothing (aka false)
             return
 
-    def _populate_traffic_managers(self):
-        self.log.debug('traffic managers: loading')
-        list_profiles = self._tm_client.profiles.list_by_resource_group
-        for profile in list_profiles(self._resource_group):
-            self._traffic_managers[profile.id] = profile
-        # link nested profiles in advance for convenience
-        for _, profile in self._traffic_managers.items():
-            self._populate_nested_profiles(profile)
-
-    def _populate_nested_profiles(self, profile):
-        for ep in profile.endpoints:
-            target_id = ep.target_resource_id
-            if target_id and target_id in self._traffic_managers:
-                target = self._traffic_managers[target_id]
-                ep.target_resource = self._populate_nested_profiles(target)
-        return profile
-
-    def _get_tm_profile_by_id(self, resource_id):
-        if not self._traffic_managers:
-            self._populate_traffic_managers()
-        return self._traffic_managers.get(resource_id)
-
-    def _profile_name_to_id(self, name):
-        return (
-            '/subscriptions/'
-            + self._client_subscription_id
-            + '/resourceGroups/'
-            + self._resource_group
-            + '/providers/Microsoft.Network/trafficManagerProfiles/'
-            + name
-        )
-
-    def _get_tm_profile_by_name(self, name):
-        profile_id = self._profile_name_to_id(name)
-        return self._get_tm_profile_by_id(profile_id)
-
-    def _get_tm_for_dynamic_record(self, record):
-        name = _root_traffic_manager_name(record)
-        return self._get_tm_profile_by_name(name)
-
     def populate(self, zone, target=False, lenient=False):
         '''Required function of manager.py to collect records from zone.
 
         Special notes for Azure.
         Azure zone names omit final '.'
         Azure root records names are represented by '@'. OctoDNS uses ''
         Azure records created through online interface may have null values
@@ -777,18 +686,19 @@
         self.log.debug('populate: name=%s', zone.name)
 
         exists = False
         before = len(zone.records)
 
         zone_name = zone.name[:-1]
 
-        records = self._dns_client.record_sets.list_by_dns_zone
         if self._check_zone(zone_name):
             exists = True
-            for azrecord in records(self._resource_group, zone_name):
+            rg = self._resource_group
+            top = self._dns_client_top
+            for azrecord in self._zone_records(rg, zone_name, top):
                 typ = _parse_azure_type(azrecord.type)
                 if typ not in self.SUPPORTS:
                     continue
 
                 record = self._populate_record(zone, azrecord, lenient)
                 zone.add_record(record, lenient=lenient)
 
@@ -813,43 +723,17 @@
         data_for = getattr(self, f'_data_for_{typ}')
         data = data_for(azrecord)
         data['type'] = typ
         data['ttl'] = azrecord.ttl
         return Record.new(zone, record_name, data, source=self, lenient=lenient)
 
     def _data_for_A(self, azrecord):
-        if azrecord.a_records is None:
-            if azrecord.target_resource.id:
-                return self._data_for_dynamic(azrecord)
-
-            # dynamic record alias is broken, return dummy value and apply
-            # will likely overwrite/fix it
-            self.log.warning(
-                '_data_for_A: Missing Traffic Manager alias for '
-                'dynamic record %s',
-                azrecord.fqdn,
-            )
-            return {'values': []}
-
         return {'values': [ar.ipv4_address for ar in azrecord.a_records]}
 
     def _data_for_AAAA(self, azrecord):
-        if azrecord.aaaa_records is None:
-            if azrecord.target_resource.id:
-                return self._data_for_dynamic(azrecord)
-
-            # dynamic record alias is broken, return dummy value and apply
-            # will likely overwrite/fix it
-            self.log.warning(
-                '_data_for_AAAA: Missing Traffic Manager alias '
-                'for dynamic record %s',
-                azrecord.fqdn,
-            )
-            return {'values': []}
-
         return {'values': [ar.ipv6_address for ar in azrecord.aaaa_records]}
 
     def _data_for_CAA(self, azrecord):
         return {
             'values': [
                 {'flags': ar.flags, 'tag': ar.tag, 'value': ar.value}
                 for ar in azrecord.caa_records
@@ -859,27 +743,14 @@
     def _data_for_CNAME(self, azrecord):
         '''Parsing data from Azure DNS Client record call
         :param azrecord: a return of a call to list azure records
         :type  azrecord: azure.mgmt.dns.models.RecordSet
 
         :type  return: dict
         '''
-        if azrecord.cname_record is None:
-            if azrecord.target_resource.id:
-                return self._data_for_dynamic(azrecord)
-
-            # dynamic record alias is broken, return dummy value and apply
-            # will likely overwrite/fix it
-            self.log.warning(
-                '_data_for_CNAME: Missing Traffic Manager alias '
-                'for dynamic record %s',
-                azrecord.fqdn,
-            )
-            return {'value': None}
-
         return {'value': _check_endswith_dot(azrecord.cname_record.cname)}
 
     def _data_for_MX(self, azrecord):
         return {
             'values': [
                 {'preference': ar.preference, 'exchange': ar.exchange}
                 for ar in azrecord.mx_records
@@ -911,14 +782,256 @@
         return {
             'values': [
                 escape_semicolon(reduce((lambda a, b: a + b), ar.value))
                 for ar in azrecord.txt_records
             ]
         }
 
+    def _apply_Delete(self, change):
+        '''A record from change must be deleted.
+
+        :param change: a change object
+        :type  change: octodns.record.Change
+
+        :type return: void
+        '''
+        record = change.existing
+        ar = _AzureRecord(self._resource_group, record, delete=True)
+
+        self._delete_record(
+            self._resource_group,
+            ar.zone_name,
+            ar.relative_record_set_name,
+            ar.record_type,
+        )
+
+        self.log.debug('*  Success Delete: %s', record)
+
+    def _apply(self, plan):
+        '''Required function of manager.py to actually apply a record change.
+
+        :param plan: Contains the zones and changes to be made
+        :type  plan: octodns.provider.base.Plan
+
+        :type return: void
+        '''
+        desired = plan.desired
+        changes = plan.changes
+        self.log.debug(
+            '_apply: zone=%s, len(changes)=%d', desired.name, len(changes)
+        )
+
+        azure_zone_name = desired.name[: len(desired.name) - 1]
+        self._check_zone(azure_zone_name, create=True)
+
+        '''
+        Force the operation order to be Delete() before all other operations.
+        Helps avoid problems in updating
+            - a CNAME record into an A record.
+            - an A record into a CNAME record.
+        '''
+
+        for change in changes:
+            class_name = change.__class__.__name__
+            if class_name == 'Delete':
+                self._apply_Delete(change)
+
+        for change in changes:
+            class_name = change.__class__.__name__
+            if class_name == 'Delete':
+                continue
+            getattr(self, f'_apply_{class_name}')(change)
+
+
+class AzureProvider(AzureBaseProvider):
+    '''
+    Azure DNS Provider
+
+    azuredns.py:
+        class: octodns_azure.AzureProvider
+        # Current support of authentication of access to Azure services only
+        # includes using a Service Principal:
+        # https://docs.microsoft.com/en-us/azure/azure-resource-manager/
+        #                        resource-group-create-service-principal-portal
+        # The Azure Active Directory Application ID (aka client ID):
+        client_id:
+        # Authentication Key Value: (note this should be secret)
+        key:
+        # Directory ID (aka tenant ID):
+        directory_id:
+        # Subscription ID:
+        sub_id:
+        # Resource Group name:
+        resource_group:
+        # All are required to authenticate.
+        #
+        # The maximum number of record sets to return per page.
+        # https://learn.microsoft.com/en-us/rest/api/dns/record-sets/list-by-dns-zone
+        # Top default 100
+        top: 100
+
+        Example config file with variables:
+            "
+            ---
+            providers:
+              config:
+                class: octodns.provider.yaml.YamlProvider
+                directory: ./config (example path to directory of zone files)
+              azuredns:
+                class: octodns_azure.AzureProvider
+                client_id: env/AZURE_APPLICATION_ID
+                key: env/AZURE_AUTHENTICATION_KEY
+                directory_id: env/AZURE_DIRECTORY_ID
+                sub_id: env/AZURE_SUBSCRIPTION_ID
+                resource_group: 'TestResource1'
+                top: 500
+
+            zones:
+              example.com.:
+                sources:
+                  - config
+                targets:
+                  - azuredns
+            "
+        The first four variables above can be hidden in environment variables
+        and octoDNS will automatically search for them in the shell. It is
+        possible to also hard-code into the config file: eg, resource_group.
+
+        Please read https://github.com/octodns/octodns/pull/706 for an overview
+        of how dynamic records are designed and caveats of using them.
+    '''
+
+    SUPPORTS_ROOT_NS = True
+    SUPPORTS_DYNAMIC = True
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.__tm_client = None
+
+    @property
+    def dns_client(self):
+        if self._dns_client is None:
+            self._dns_client = DnsManagementClient(
+                credential=self._client_credential,
+                subscription_id=self._client_subscription_id,
+                retry_policy=self._dns_client_retry_policy,
+                base_url=self._base_url,
+            )
+        return self._dns_client
+
+    @property
+    def _tm_client(self):
+        if self.__tm_client is None:
+            self.__tm_client = TrafficManagerManagementClient(
+                credential=self._client_credential,
+                subscription_id=self._client_subscription_id,
+                base_url=self._base_url,
+            )
+        return self.__tm_client
+
+    def _dns_client_zones(self):
+        return self.dns_client.zones
+
+    def _create_zone(self, name):
+        create_zone = self.dns_client.zones.create_or_update
+        return create_zone(self._resource_group, name, Zone(location='global'))
+
+    def _zone_records(self, resource_group, name, top):
+        return self.dns_client.record_sets.list_by_dns_zone(
+            resource_group, name, top
+        )
+
+    def _populate_traffic_managers(self):
+        self.log.debug('traffic managers: loading')
+        list_profiles = self._tm_client.profiles.list_by_resource_group
+        for profile in list_profiles(self._resource_group):
+            self._traffic_managers[profile.id] = profile
+        # link nested profiles in advance for convenience
+        for _, profile in self._traffic_managers.items():
+            self._populate_nested_profiles(profile)
+
+    def _populate_nested_profiles(self, profile):
+        for ep in profile.endpoints:
+            target_id = ep.target_resource_id
+            if target_id and target_id in self._traffic_managers:
+                target = self._traffic_managers[target_id]
+                ep.target_resource = self._populate_nested_profiles(target)
+        return profile
+
+    def _get_tm_profile_by_id(self, resource_id):
+        if not self._traffic_managers:
+            self._populate_traffic_managers()
+        return self._traffic_managers.get(resource_id)
+
+    def _profile_name_to_id(self, name):
+        return (
+            '/subscriptions/'
+            + self._client_subscription_id
+            + '/resourceGroups/'
+            + self._resource_group
+            + '/providers/Microsoft.Network/trafficManagerProfiles/'
+            + name
+        )
+
+    def _get_tm_profile_by_name(self, name):
+        profile_id = self._profile_name_to_id(name)
+        return self._get_tm_profile_by_id(profile_id)
+
+    def _get_tm_for_dynamic_record(self, record):
+        name = _root_traffic_manager_name(record)
+        return self._get_tm_profile_by_name(name)
+
+    def _data_for_A(self, azrecord):
+        if azrecord.a_records is None:
+            if azrecord.target_resource.id:
+                return self._data_for_dynamic(azrecord)
+
+            # dynamic record alias is broken, return dummy value and apply
+            # will likely overwrite/fix it
+            self.log.warning(
+                '_data_for_A: Missing Traffic Manager alias for '
+                'dynamic record %s',
+                azrecord.fqdn,
+            )
+            return {'values': []}
+
+        return super()._data_for_A(azrecord)
+
+    def _data_for_AAAA(self, azrecord):
+        if azrecord.aaaa_records is None:
+            if azrecord.target_resource.id:
+                return self._data_for_dynamic(azrecord)
+
+            # dynamic record alias is broken, return dummy value and apply
+            # will likely overwrite/fix it
+            self.log.warning(
+                '_data_for_AAAA: Missing Traffic Manager alias '
+                'for dynamic record %s',
+                azrecord.fqdn,
+            )
+            return {'values': []}
+
+        return super()._data_for_AAAA(azrecord)
+
+    def _data_for_CNAME(self, azrecord):
+        if azrecord.cname_record is None:
+            if azrecord.target_resource.id:
+                return self._data_for_dynamic(azrecord)
+
+            # dynamic record alias is broken, return dummy value and apply
+            # will likely overwrite/fix it
+            self.log.warning(
+                '_data_for_CNAME: Missing Traffic Manager alias '
+                'for dynamic record %s',
+                azrecord.fqdn,
+            )
+            return {'value': None}
+
+        return super()._data_for_CNAME(azrecord)
+
     def _get_geo_endpoints(self, root_profile):
         if root_profile.traffic_routing_method != 'Geographic':
             # This record does not use geo fencing, so we skip the Geographic
             # profile hop; let's pretend to be a geo-profile's only endpoint
             geo_ep = Endpoint(
                 name=root_profile.endpoints[0].name.split('--', 1)[0],
                 target_resource_id=root_profile.id,
@@ -1001,17 +1114,17 @@
                 val = _check_endswith_dot(val)
 
             ep_name = pool_ep.name
             if ep_name.endswith('--default--'):
                 defaults.add(val)
                 ep_name = ep_name[: -len('--default--')]
 
-            status = 'obey'
-            if pool_ep.endpoint_status == 'Disabled':
-                status = 'down'
+            status = _endpoint_flags_to_value_status(
+                pool_ep.endpoint_status, pool_ep.always_serve
+            )
 
             values.append(
                 {'value': val, 'weight': pool_ep.weight or 1, 'status': status}
             )
 
         return values
 
@@ -1136,40 +1249,14 @@
                     msg = (
                         'required azure-dns.* root NS values missing '
                         + f'from {record.fqdn}'
                     )
                     fallback = 'adding them'
                     self.supports_warn_or_except(msg, fallback)
                     desired.add_record(record, replace=True)
-            elif getattr(record, 'dynamic', False):
-                # check for status=up values
-                up_pools = []
-                for name, pool in record.dynamic.pools.items():
-                    for value in pool.data['values']:
-                        if value['status'] == 'up':
-                            # Azure only supports obey and down, not up
-                            up_pools.append(name)
-                            break
-                if not up_pools:
-                    continue
-
-                up_pools = ','.join(up_pools)
-                msg = (
-                    f'status=up is not supported for pools {up_pools} in '
-                    f'{record.fqdn}'
-                )
-                fallback = 'will ignore it and respect the healthcheck'
-                self.supports_warn_or_except(msg, fallback)
-
-                record = record.copy()
-                for pool in record.dynamic.pools.values():
-                    for value in pool.data['values']:
-                        if value['status'] == 'up':
-                            value['status'] = 'obey'
-                desired.add_record(record, replace=True)
 
         return super()._process_desired_zone(desired)
 
     def _extra_changes(self, existing, desired, changes):
         changed = set(c.record for c in changes)
 
         log = self.log.info
@@ -1303,24 +1390,27 @@
             target = val['value']
             # strip trailing dot from CNAME value
             if record._type == 'CNAME':
                 target = target[:-1]
             ep_name = f'{pool_name}--{target}'
             # Endpoint names cannot have colons, drop them from IPv6 addresses
             ep_name = ep_name.replace(':', '-')
-            ep_status = 'Disabled' if val['status'] == 'down' else 'Enabled'
-            if val['value'] in defaults:
+            ep_status, always_serve = _value_status_to_endpoint_flags(
+                val['status']
+            )
+            if val['value'] in defaults and val['status'] == 'up':
                 # mark default
                 ep_name += '--default--'
             endpoints.append(
                 Endpoint(
                     name=ep_name,
                     target=target,
                     weight=val.get('weight', 1),
                     endpoint_status=ep_status,
+                    always_serve=always_serve,
                 )
             )
 
         return self._generate_tm_profile(
             'Weighted', endpoints, record, pool_name
         )
 
@@ -1328,22 +1418,21 @@
         self, pool, priority, pool_profiles, record, defaults, traffic_managers
     ):
         pool_name = pool._id
         pool_values = pool.data['values']
         first_value = pool_values[0]
 
         if len(pool_values) > 1 or (
-            first_value['value'] in defaults and first_value['status'] != 'obey'
+            first_value['value'] in defaults and first_value['status'] != 'up'
         ):
             # create Weighted profile for multi-value pool
             #
-            # or if a single-value pool has the default as its member and isn't enabled
+            # or if a single-value pool has the default as its member and it's status is not 'up'
             # ^^ is because a TM profile does not allow multiple endpoints for the same FQDN, so we
             # branch off into a nested profile so we can add the default as the last priority endpoint.
-            # TODO: change `status!=obey` conditional to `status!=up` when the support lands
             pool_profile = pool_profiles.get(pool_name)
             if not pool_profile:
                 pool_profile = self._make_pool_profile(pool, record, defaults)
                 traffic_managers.append(pool_profile)
                 pool_profiles[pool_name] = pool_profile
 
             # append pool to endpoint list of fallback rule profile
@@ -1353,27 +1442,30 @@
                 priority=priority,
             )
         else:
             # Skip Weighted profile hop for single-value pool; append its
             # value as an external endpoint to fallback rule profile
             value = pool_values[0]
             ep_name = pool_name
-            ep_status = 'Disabled' if value['status'] == 'down' else 'Enabled'
+            ep_status, always_serve = _value_status_to_endpoint_flags(
+                value['status']
+            )
             target = value['value']
             if target in defaults:
                 # mark default
                 ep_name += '--default--'
             # strip trailing dot from CNAME value
             if record._type == 'CNAME':
                 target = target[:-1]
             return Endpoint(
                 name=ep_name,
                 target=target,
                 priority=priority,
                 endpoint_status=ep_status,
+                always_serve=always_serve,
             )
 
     def _make_rule_profile(
         self, rule_endpoints, rule_name, record, geos, traffic_managers
     ):
         if len(rule_endpoints) > 1:
             # create rule profile with fallback chain
@@ -1402,14 +1494,15 @@
             else:
                 # just add the value of single-value pool
                 return Endpoint(
                     name=rule_ep.name,
                     target=rule_ep.target,
                     geo_mapping=geos,
                     endpoint_status=rule_ep.endpoint_status,
+                    always_serve=rule_ep.always_serve,
                 )
 
     def _make_rule(
         self, pool_name, pool_profiles, record, geos, traffic_managers
     ):
         endpoints = []
         rule_name = pool_name
@@ -1433,32 +1526,37 @@
                 record,
                 defaults,
                 traffic_managers,
             )
             endpoints.append(rule_ep)
 
             if not default_seen and any(
-                val['value'] in defaults and val['status'] == 'obey'
+                val['value'] in defaults and val['status'] == 'up'
                 for val in pool.data['values']
             ):
-                # TODO: change `status=obey` conditional to `status=up` when the support lands
                 default_seen = True
 
             priority += 1
             pool_name = pool.data.get('fallback')
 
-        # append default endpoint unless it is already included in last pool
-        # of rule profile
+        # append default endpoint unless it is already included in a pool with status=up
         if not default_seen:
             default = defaults[0]
             if record._type == 'CNAME':
                 default = default[:-1]
-            # TODO: set status=up when the support lands
+            # default should always be up
+            ep_status, always_serve = _value_status_to_endpoint_flags('up')
             endpoints.append(
-                Endpoint(name='--default--', target=default, priority=priority)
+                Endpoint(
+                    name='--default--',
+                    target=default,
+                    priority=priority,
+                    endpoint_status=ep_status,
+                    always_serve=always_serve,
+                )
             )
 
         return self._make_rule_profile(
             endpoints, rule_name, record, geos, traffic_managers
         )
 
     def _make_geo_rules(self, record):
@@ -1515,67 +1613,14 @@
             geo_profile = self._generate_tm_profile(
                 'Geographic', geo_endpoints, record
             )
             traffic_managers.append(geo_profile)
 
         return traffic_managers
 
-    def _sync_traffic_managers(self, desired_profiles):
-        seen = set()
-
-        tm_sync = self._tm_client.profiles.create_or_update
-        populate = self._populate_nested_profiles
-
-        for desired in desired_profiles:
-            name = desired.name
-            if name in seen:
-                continue
-
-            existing = self._get_tm_profile_by_name(name)
-            if not _profile_is_match(existing, desired):
-                self.log.info(
-                    '_sync_traffic_managers: Syncing profile=%s', name
-                )
-                profile = tm_sync(self._resource_group, name, desired)
-                self._traffic_managers[profile.id] = populate(profile)
-            else:
-                self.log.debug(
-                    '_sync_traffic_managers: Skipping profile=%s: up to date',
-                    name,
-                )
-            seen.add(name)
-
-        return seen
-
-    def _find_traffic_managers(self, record):
-        tm_prefix = _root_traffic_manager_name(record)
-
-        profiles = set()
-        for profile_id in self._traffic_managers:
-            # match existing profiles with record's prefix
-            name = profile_id.split('/')[-1]
-            if (
-                name == tm_prefix
-                or name.startswith(f'{tm_prefix}-pool-')
-                or name.startswith(f'{tm_prefix}-rule-')
-            ):
-                profiles.add(name)
-
-        return profiles
-
-    def _traffic_managers_gc(self, record, active_profiles):
-        existing_profiles = self._find_traffic_managers(record)
-
-        # delete unused profiles
-        for profile_name in existing_profiles - active_profiles:
-            self.log.info(
-                '_traffic_managers_gc: Deleting profile=%s', profile_name
-            )
-            self._tm_client.profiles.delete(self._resource_group, profile_name)
-
     def _apply_Create(self, change):
         '''A record from change must be created.
 
         :param change: a change object
         :type  change: octodns.record.Change
 
         :type return: void
@@ -1609,16 +1654,16 @@
                 endpoints = root_profile.endpoints
                 root_profile.endpoints = []
             self._sync_traffic_managers(profiles)
 
         ar = _AzureRecord(
             self._resource_group, record, traffic_manager=root_profile
         )
-        create = self._dns_client.record_sets.create_or_update
 
+        create = self.dns_client.record_sets.create_or_update
         create(
             resource_group_name=ar.resource_group,
             zone_name=ar.zone_name,
             relative_record_set_name=ar.relative_record_set_name,
             record_type=ar.record_type,
             parameters=ar.params,
         )
@@ -1627,14 +1672,67 @@
             # add nested endpoints for A/AAAA dynamic record limitation after
             # record creation
             root_profile.endpoints = endpoints
             self._sync_traffic_managers([root_profile])
 
         self.log.debug('*  Success Create: %s', record)
 
+    def _sync_traffic_managers(self, desired_profiles):
+        seen = set()
+
+        tm_sync = self._tm_client.profiles.create_or_update
+        populate = self._populate_nested_profiles
+
+        for desired in desired_profiles:
+            name = desired.name
+            if name in seen:
+                continue
+
+            existing = self._get_tm_profile_by_name(name)
+            if not _profile_is_match(existing, desired):
+                self.log.info(
+                    '_sync_traffic_managers: Syncing profile=%s', name
+                )
+                profile = tm_sync(self._resource_group, name, desired)
+                self._traffic_managers[profile.id] = populate(profile)
+            else:
+                self.log.debug(
+                    '_sync_traffic_managers: Skipping profile=%s: up to date',
+                    name,
+                )
+            seen.add(name)
+
+        return seen
+
+    def _find_traffic_managers(self, record):
+        tm_prefix = _root_traffic_manager_name(record)
+
+        profiles = set()
+        for profile_id in self._traffic_managers:
+            # match existing profiles with record's prefix
+            name = profile_id.split('/')[-1]
+            if (
+                name == tm_prefix
+                or name.startswith(f'{tm_prefix}-pool-')
+                or name.startswith(f'{tm_prefix}-rule-')
+            ):
+                profiles.add(name)
+
+        return profiles
+
+    def _traffic_managers_gc(self, record, active_profiles):
+        existing_profiles = self._find_traffic_managers(record)
+
+        # delete unused profiles
+        for profile_name in existing_profiles - active_profiles:
+            self.log.info(
+                '_traffic_managers_gc: Deleting profile=%s', profile_name
+            )
+            self._tm_client.profiles.delete(self._resource_group, profile_name)
+
     def _apply_Update(self, change):
         '''A record from change must be created.
 
         :param change: a change object
         :type  change: octodns.record.Change
 
         :type return: void
@@ -1670,16 +1768,16 @@
             active = self._sync_traffic_managers(profiles)
 
         if update_record:
             profile = self._get_tm_for_dynamic_record(new)
             ar = _AzureRecord(
                 self._resource_group, new, traffic_manager=profile
             )
-            update = self._dns_client.record_sets.create_or_update
 
+            update = self.dns_client.record_sets.create_or_update
             update(
                 resource_group_name=ar.resource_group,
                 zone_name=ar.zone_name,
                 relative_record_set_name=ar.relative_record_set_name,
                 record_type=ar.record_type,
                 parameters=ar.params,
             )
@@ -1695,64 +1793,162 @@
             # cleanup traffic managers when a dynamic record gets
             # changed to a simple record
             self._traffic_managers_gc(existing, set())
 
         self.log.debug('*  Success Update: %s', new)
 
     def _apply_Delete(self, change):
-        '''A record from change must be deleted.
+        record = change.existing
+        super()._apply_Delete(change)
+
+        if getattr(record, 'dynamic', False):
+            self._traffic_managers_gc(record, set())
+
+    def _delete_record(
+        self, resource_group, zone_name, relative_record_set_name, record_type
+    ):
+        delete = self.dns_client.record_sets.delete
+        delete(resource_group, zone_name, relative_record_set_name, record_type)
+
+
+class AzurePrivateProvider(AzureBaseProvider):
+    '''
+    Azure DNS Provider
+
+    azuredns.py:
+        class: octodns_azure.AzurePrivateProvider
+        # Current support of authentication of access to Azure services only
+        # includes using a Service Principal:
+        # https://docs.microsoft.com/en-us/azure/azure-resource-manager/
+        #                        resource-group-create-service-principal-portal
+        # The Azure Active Directory Application ID (aka client ID):
+        client_id:
+        # Authentication Key Value: (note this should be secret)
+        key:
+        # Directory ID (aka tenant ID):
+        directory_id:
+        # Subscription ID:
+        sub_id:
+        # Resource Group name:
+        resource_group:
+        # All are required to authenticate.
+        #
+        # The maximum number of record sets to return per page.
+        # https://learn.microsoft.com/en-us/rest/api/dns/record-sets/list-by-dns-zone
+        # Top default 100
+        top: 100
+
+        Example config file with variables:
+            "
+            ---
+            providers:
+              config:
+                class: octodns.provider.yaml.YamlProvider
+                directory: ./config (example path to directory of zone files)
+              azuredns:
+                class: octodns_azure.AzurePrivateProvider
+                client_id: env/AZURE_APPLICATION_ID
+                key: env/AZURE_AUTHENTICATION_KEY
+                directory_id: env/AZURE_DIRECTORY_ID
+                sub_id: env/AZURE_SUBSCRIPTION_ID
+                resource_group: 'TestResource1'
+                top: 500
+
+            zones:
+              example.com.:
+                sources:
+                  - config
+                targets:
+                  - azuredns
+            "
+        The first four variables above can be hidden in environment variables
+        and octoDNS will automatically search for them in the shell. It is
+        possible to also hard-code into the config file: eg, resource_group.
+
+        Please read https://github.com/octodns/octodns/pull/706 for an overview
+        of how dynamic records are designed and caveats of using them.
+    '''
+
+    # private dns doesn't support name_servers
+    # https://learn.microsoft.com/en-us/python/api/azure-mgmt-privatedns/azure.mgmt.privatedns.models.privatezone?view=azure-python
+    SUPPORTS_ROOT_NS = False
+    # If enabled this would create public traffic managers which doesn't make
+    # sense.
+    SUPPORTS_DYNAMIC = False
+
+    @property
+    def dns_client(self):
+        if self._dns_client is None:
+            self._dns_client = PrivateDnsManagementClient(
+                credential=self._client_credential,
+                subscription_id=self._client_subscription_id,
+                base_url=self._base_url,
+            )
+        return self._dns_client
+
+    def _dns_client_zones(self):
+        return self.dns_client.private_zones
+
+    def _create_zone(self, name):
+        create_zone = self.dns_client.private_zones._create_or_update_initial
+        return create_zone(
+            self._resource_group, name, PrivateZone(location='global')
+        )
+
+    def _zone_records(self, resource_group, name, top):
+        return self.dns_client.record_sets.list(resource_group, name, top)
+
+    def _apply_Create(self, change):
+        '''A record from change must be created.
 
         :param change: a change object
         :type  change: octodns.record.Change
 
         :type return: void
         '''
-        record = change.record
-        ar = _AzureRecord(self._resource_group, record, delete=True)
-        delete = self._dns_client.record_sets.delete
+        record = change.new
+        ar = _AzureRecord(self._resource_group, record)
 
-        delete(
-            self._resource_group,
-            ar.zone_name,
-            ar.relative_record_set_name,
-            ar.record_type,
+        create = self.dns_client.record_sets.create_or_update
+        create(
+            resource_group_name=ar.resource_group,
+            private_zone_name=ar.zone_name,
+            relative_record_set_name=ar.relative_record_set_name,
+            record_type=ar.record_type,
+            parameters=ar.params,
         )
 
-        if getattr(record, 'dynamic', False):
-            self._traffic_managers_gc(record, set())
-
-        self.log.debug('*  Success Delete: %s', record)
+        self.log.debug('*  Success Create: %s', record)
 
-    def _apply(self, plan):
-        '''Required function of manager.py to actually apply a record change.
+    def _apply_Update(self, change):
+        '''A record from change must be created.
 
-        :param plan: Contains the zones and changes to be made
-        :type  plan: octodns.provider.base.Plan
+        :param change: a change object
+        :type  change: octodns.record.Change
 
         :type return: void
         '''
-        desired = plan.desired
-        changes = plan.changes
-        self.log.debug(
-            '_apply: zone=%s, len(changes)=%d', desired.name, len(changes)
-        )
-
-        azure_zone_name = desired.name[: len(desired.name) - 1]
-        self._check_zone(azure_zone_name, create=True)
+        new = change.new
+        ar = _AzureRecord(self._resource_group, new)
 
-        '''
-        Force the operation order to be Delete() before all other operations.
-        Helps avoid problems in updating
-            - a CNAME record into an A record.
-            - an A record into a CNAME record.
-        '''
+        update = self.dns_client.record_sets.create_or_update
+        update(
+            resource_group_name=ar.resource_group,
+            private_zone_name=ar.zone_name,
+            relative_record_set_name=ar.relative_record_set_name,
+            record_type=ar.record_type,
+            parameters=ar.params,
+        )
 
-        for change in changes:
-            class_name = change.__class__.__name__
-            if class_name == 'Delete':
-                self._apply_Delete(change)
+        self.log.debug('*  Success Update: %s', new)
 
-        for change in changes:
-            class_name = change.__class__.__name__
-            if class_name == 'Delete':
-                continue
-            getattr(self, f'_apply_{class_name}')(change)
+    def _delete_record(
+        self, resource_group, zone_name, relative_record_set_name, record_type
+    ):
+        delete = self.dns_client.record_sets.delete
+        delete(
+            resource_group,
+            zone_name,
+            # these last 2 parms seem flipped from the non-private version
+            record_type,
+            relative_record_set_name,
+        )
```

### Comparing `octodns-azure-0.0.4/octodns_azure.egg-info/PKG-INFO` & `octodns-azure-0.0.5/octodns_azure.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: octodns-azure
-Version: 0.0.4
+Version: 0.0.5
 Summary:  Azure DNS & TrafficManager provider for octoDNS
 Home-page: https://github.com/octodns/octodns-azure
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 
 ## Azure DNS & TrafficManager provider for octoDNS
 
 An [octoDNS](https://github.com/octodns/octodns/) provider that targets [Azure](https://azure.microsoft.com/en-us/services/dns/#overview).
@@ -66,18 +66,24 @@
     # All are required to authenticate.
     # Azure RetryPolicy Settings all of them are optional.
     # https://azuresdkdocs.blob.core.windows.net/$web/python/azure-core/1.9.0/azure.core.pipeline.policies.html?highlight=retrypolicy#azure.core.pipeline.policies.RetryPolicy
     # Total_retries default 10
     #client_total_retries: 10
     # status_retries default 3
     #client_status_retries: 3
+    # The maximum number of record sets to return per page.
+    # https://learn.microsoft.com/en-us/rest/api/dns/record-sets/list-by-dns-zone
+    # Top default 100
+    #top: 100
 ```
 
 The first four variables above can be hidden in environment variables and octoDNS will automatically search for them in the shell. It is possible to also hard-code into the config file: eg, resource_group.
 
+For management of DNS zones on [Azure Private DNS](https://learn.microsoft.com/en-us/azure/dns/private-dns-overview), use `class: octodns_azure.AzurePrivateProvider`. Note that this provider does not support dynamic records or root NS records.
+
 ### Support Information
 
 #### Records
 
 AzureProvider supports A, AAAA, CAA, CNAME, MX, NS, PTR, SRV, and TXT
 
 #### Root NS Records
@@ -101,15 +107,15 @@
 | num_failures | This value specifies how many failures a Traffic Manager probing agent tolerates before marking that endpoint as unhealthy. Its value can range between 0 and 9. A value of 0 means a single monitoring failure can cause that endpoint to be marked as unhealthy. If no value is specified, it uses the default value of 3. | 3 |
 
 ```
 ---
   octodns:
     azuredns:
       healthcheck:
-        interval_in_seconds: 10
-        timeout_in_seconds: 7
-        tolerated_number_of_failures: 4
+        interval: 10
+        timeout: 7
+        num_failures: 4
 ```
 
 ### Development
 
 See the [/script/](/script/) directory for some tools to help with the development process. They generally follow the [Script to rule them all](https://github.com/github/scripts-to-rule-them-all) pattern. Most useful is `./script/bootstrap` which will create a venv and install both the runtime and development related requirements. It will also hook up a pre-commit hook that covers most of what's run by CI.
```

