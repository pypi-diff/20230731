# Comparing `tmp/octodns-ns1-0.0.4.tar.gz` & `tmp/octodns-ns1-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns-ns1-0.0.4.tar", last modified: Thu Apr  6 23:32:51 2023, max compression
+gzip compressed data, was "octodns-ns1-0.0.5.tar", last modified: Mon Jul 31 18:04:03 2023, max compression
```

## Comparing `octodns-ns1-0.0.4.tar` & `octodns-ns1-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-04-06 23:32:51.501676 octodns-ns1-0.0.4/
--rw-r--r--   0 ross       (501) staff       (20)     4428 2023-04-06 23:32:51.501403 octodns-ns1-0.0.4/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)     4115 2023-04-06 18:12:34.000000 octodns-ns1-0.0.4/README.md
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-04-06 23:32:51.498350 octodns-ns1-0.0.4/octodns_ns1/
--rw-r--r--   0 ross       (501) staff       (20)    58598 2023-04-06 23:32:37.000000 octodns-ns1-0.0.4/octodns_ns1/__init__.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-04-06 23:32:51.500595 octodns-ns1-0.0.4/octodns_ns1.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)     4428 2023-04-06 23:32:51.000000 octodns-ns1-0.0.4/octodns_ns1.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      258 2023-04-06 23:32:51.000000 octodns-ns1-0.0.4/octodns_ns1.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2023-04-06 23:32:51.000000 octodns-ns1-0.0.4/octodns_ns1.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)      254 2023-04-06 23:32:51.000000 octodns-ns1-0.0.4/octodns_ns1.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       12 2023-04-06 23:32:51.000000 octodns-ns1-0.0.4/octodns_ns1.egg-info/top_level.txt
--rw-r--r--   0 ross       (501) staff       (20)      304 2023-02-04 19:09:21.000000 octodns-ns1-0.0.4/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)       38 2023-04-06 23:32:51.501763 octodns-ns1-0.0.4/setup.cfg
--rw-r--r--   0 ross       (501) staff       (20)     1814 2023-02-04 19:09:21.000000 octodns-ns1-0.0.4/setup.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-04-06 23:32:51.500899 octodns-ns1-0.0.4/tests/
--rw-r--r--   0 ross       (501) staff       (20)   105009 2023-04-06 18:41:05.000000 octodns-ns1-0.0.4/tests/test_provider_ns1.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-07-31 18:04:03.240495 octodns-ns1-0.0.5/
+-rw-r--r--   0 neo       (1000) neo       (1000)     4950 2023-07-31 18:04:03.240495 octodns-ns1-0.0.5/PKG-INFO
+-rw-r--r--   0 neo       (1000) neo       (1000)     4637 2023-07-26 10:22:02.000000 octodns-ns1-0.0.5/README.md
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-07-31 18:04:03.237162 octodns-ns1-0.0.5/octodns_ns1/
+-rw-r--r--   0 neo       (1000) neo       (1000)    66099 2023-07-31 17:58:22.000000 octodns-ns1-0.0.5/octodns_ns1/__init__.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-07-31 18:04:03.237162 octodns-ns1-0.0.5/octodns_ns1.egg-info/
+-rw-r--r--   0 neo       (1000) neo       (1000)     4950 2023-07-31 18:04:03.000000 octodns-ns1-0.0.5/octodns_ns1.egg-info/PKG-INFO
+-rw-r--r--   0 neo       (1000) neo       (1000)      258 2023-07-31 18:04:03.000000 octodns-ns1-0.0.5/octodns_ns1.egg-info/SOURCES.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)        1 2023-07-31 18:04:03.000000 octodns-ns1-0.0.5/octodns_ns1.egg-info/dependency_links.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)      264 2023-07-31 18:04:03.000000 octodns-ns1-0.0.5/octodns_ns1.egg-info/requires.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       12 2023-07-31 18:04:03.000000 octodns-ns1-0.0.5/octodns_ns1.egg-info/top_level.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)      304 2023-03-26 18:48:23.000000 octodns-ns1-0.0.5/pyproject.toml
+-rw-r--r--   0 neo       (1000) neo       (1000)       38 2023-07-31 18:04:03.240495 octodns-ns1-0.0.5/setup.cfg
+-rw-r--r--   0 neo       (1000) neo       (1000)     2140 2023-07-31 17:58:22.000000 octodns-ns1-0.0.5/setup.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-07-31 18:04:03.237162 octodns-ns1-0.0.5/tests/
+-rw-r--r--   0 neo       (1000) neo       (1000)   118653 2023-07-31 18:01:36.000000 octodns-ns1-0.0.5/tests/test_provider_ns1.py
```

### Comparing `octodns-ns1-0.0.4/PKG-INFO` & `octodns-ns1-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: octodns-ns1
-Version: 0.0.4
+Version: 0.0.5
 Summary:  NS1 provider for octoDNS
 Home-page: https://github.com/octodns/octodns-ns1
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 
 ## NS1 provider for octoDNS
 
 An [octoDNS](https://github.com/octodns/octodns/) provider that targets [NS1](https://ns1.com/products/managed-dns).
@@ -70,17 +70,22 @@
     retry_count: 4
     # Optional. Default: None. Additional options or overrides passed to
     # the NS1 SDK config, as key-value pairs.
     client_config:
         endpoint: my.nsone.endpoint # Default: api.nsone.net
         ignore-ssl-errors: true     # Default: false
         follow_pagination: false    # Default: true
-    # Optional. Default: HTTP/1.0 . Default HTTP protocol to use when 
-    # health-checking dynamic record endpoints. See "Health Check Options" 
+    # Optional. Default: false. Use modern HTTP monitor (true) or the legacy
+    # HTTP-emulating TCP monitor (false) for HTTP(s) healthchecks.
+    use_http_monitors: false
+    # Optional. Default: HTTP/1.0. Default HTTP protocol to use when
+    # health-checking dynamic record endpoints. See "Health Check Options"
     # README section below to override per dynamic record.
+    # This is only supported when use_http_monitors is set to false. If it
+    # is set to true, HTTP/1.1 will be used and it cannot be changed.
     default_healthcheck_http_version: HTTP/1.0
 
 ```
 
 ### Support Information
 
 #### Records
@@ -91,26 +96,30 @@
 
 Ns1Provider supports full root NS record management.
 
 #### Dynamic
 
 Ns1Provider supports dynamic records.
 
+#### Subnet targeting
+
+Ns1Provider supports [subnet targeting](https://github.com/octodns/octodns/blob/main/docs/dynamic_records.md#subnets) in dynamic records.
+
 #### Health Check Options
 
 See https://github.com/octodns/octodns/blob/master/docs/dynamic_records.md#health-checks for information on health checking for dynamic records. Ns1Provider supports the following options:
 
 | Key  | Description | Default |
 |--|--|--|
 | policy | One of:<ol><li>`all` - down if every region is down</li><li>`quorum` - down if majority regions are down</li><li>`one` - down if any region is down</ol> | `quorum` |
 | frequency | Frequency (in seconds) of health-check | 60 |
 | connect_timeout | Timeout (in seconds) before we give up trying to connect | 2 |
 | response_timeout | Timeout (in seconds) after connecting to wait for output | 10 |
 | rapid_recheck | Enable or disable a second, automatic verification test before changing the status of a host. Enabling this option can help prevent false positives. | False |
-| http_version | Specify HTTP version to use when HTTP health-checking  a host. One of <ol><li>`HTTP/1.0`</li><li>`HTTP/1.1`</li><ol> | `HTTP/1.0` |
+| http_version | Specify HTTP version to use when HTTP health-checking a host. Only applicable if `use_http_monitors=False`. One of <ol><li>`HTTP/1.0`</li><li>`HTTP/1.1`</li><ol> | `HTTP/1.0` |
 
 ```yaml
 ---
   octodns:
     ns1:
       healthcheck:
         policy: quorum
```

### Comparing `octodns-ns1-0.0.4/README.md` & `octodns-ns1-0.0.5/octodns_ns1.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: octodns-ns1
+Version: 0.0.5
+Summary:  NS1 provider for octoDNS
+Home-page: https://github.com/octodns/octodns-ns1
+Author: Ross McFarland
+Author-email: rwmcfa1@gmail.com
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
+
 ## NS1 provider for octoDNS
 
 An [octoDNS](https://github.com/octodns/octodns/) provider that targets [NS1](https://ns1.com/products/managed-dns).
 
 ### Installation
 
 #### Command line
@@ -57,17 +70,22 @@
     retry_count: 4
     # Optional. Default: None. Additional options or overrides passed to
     # the NS1 SDK config, as key-value pairs.
     client_config:
         endpoint: my.nsone.endpoint # Default: api.nsone.net
         ignore-ssl-errors: true     # Default: false
         follow_pagination: false    # Default: true
-    # Optional. Default: HTTP/1.0 . Default HTTP protocol to use when 
-    # health-checking dynamic record endpoints. See "Health Check Options" 
+    # Optional. Default: false. Use modern HTTP monitor (true) or the legacy
+    # HTTP-emulating TCP monitor (false) for HTTP(s) healthchecks.
+    use_http_monitors: false
+    # Optional. Default: HTTP/1.0. Default HTTP protocol to use when
+    # health-checking dynamic record endpoints. See "Health Check Options"
     # README section below to override per dynamic record.
+    # This is only supported when use_http_monitors is set to false. If it
+    # is set to true, HTTP/1.1 will be used and it cannot be changed.
     default_healthcheck_http_version: HTTP/1.0
 
 ```
 
 ### Support Information
 
 #### Records
@@ -78,26 +96,30 @@
 
 Ns1Provider supports full root NS record management.
 
 #### Dynamic
 
 Ns1Provider supports dynamic records.
 
+#### Subnet targeting
+
+Ns1Provider supports [subnet targeting](https://github.com/octodns/octodns/blob/main/docs/dynamic_records.md#subnets) in dynamic records.
+
 #### Health Check Options
 
 See https://github.com/octodns/octodns/blob/master/docs/dynamic_records.md#health-checks for information on health checking for dynamic records. Ns1Provider supports the following options:
 
 | Key  | Description | Default |
 |--|--|--|
 | policy | One of:<ol><li>`all` - down if every region is down</li><li>`quorum` - down if majority regions are down</li><li>`one` - down if any region is down</ol> | `quorum` |
 | frequency | Frequency (in seconds) of health-check | 60 |
 | connect_timeout | Timeout (in seconds) before we give up trying to connect | 2 |
 | response_timeout | Timeout (in seconds) after connecting to wait for output | 10 |
 | rapid_recheck | Enable or disable a second, automatic verification test before changing the status of a host. Enabling this option can help prevent false positives. | False |
-| http_version | Specify HTTP version to use when HTTP health-checking  a host. One of <ol><li>`HTTP/1.0`</li><li>`HTTP/1.1`</li><ol> | `HTTP/1.0` |
+| http_version | Specify HTTP version to use when HTTP health-checking a host. Only applicable if `use_http_monitors=False`. One of <ol><li>`HTTP/1.0`</li><li>`HTTP/1.1`</li><ol> | `HTTP/1.0` |
 
 ```yaml
 ---
   octodns:
     ns1:
       healthcheck:
         policy: quorum
```

### Comparing `octodns-ns1-0.0.4/octodns_ns1/__init__.py` & `octodns-ns1-0.0.5/octodns_ns1/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from pycountry_convert import country_alpha2_to_continent_code
 
 from octodns.provider import ProviderException
 from octodns.provider.base import BaseProvider
 from octodns.record import Record, Update
 from octodns.record.geo_data import geo_data
 
-__VERSION__ = '0.0.4'
+__VERSION__ = '0.0.5'
 
 
 def _ensure_endswith_dot(string):
     return string if string.endswith('.') else f'{string}.'
 
 
 class Ns1Exception(ProviderException):
@@ -281,14 +281,15 @@
                 tries -= 1
 
 
 class Ns1Provider(BaseProvider):
     SUPPORTS_GEO = True
     SUPPORTS_DYNAMIC = True
     SUPPORTS_POOL_VALUE_STATUS = True
+    SUPPORTS_DYNAMIC_SUBNETS = True
     SUPPORTS_MULTIVALUE_PTR = True
     SUPPORTS_ROOT_NS = True
     SUPPORTS = set(
         (
             'A',
             'AAAA',
             'ALIAS',
@@ -322,14 +323,21 @@
     @property
     def _COUNTRY_FILTER(self):
         return {
             'config': {'remove_no_location': True},
             'filter': u'geofence_country',
         }
 
+    @property
+    def _SUBNET_FILTER(self):
+        return {
+            'config': {'remove_no_ip_prefixes': True},
+            'filter': u'netfence_prefix',
+        }
+
     # In the NS1 UI/portal, this filter is called "SELECT FIRST GROUP" though
     # the filter name in the NS1 api is 'select_first_region'
     @property
     def _SELECT_FIRST_REGION_FILTER(self):
         return {'config': {}, 'filter': u'select_first_region'}
 
     @property
@@ -373,25 +381,73 @@
             self._SELECT_FIRST_REGION_FILTER,
             self._PRIORITY_FILTER,
             self._WEIGHTED_SHUFFLE_FILTER,
             self._SELECT_FIRST_N_FILTER,
         ]
 
     @property
+    def _FILTER_CHAIN_WITH_SUBNET(self):
+        return [
+            self._UP_FILTER,
+            self._SUBNET_FILTER,
+            self._SELECT_FIRST_REGION_FILTER,
+            self._PRIORITY_FILTER,
+            self._WEIGHTED_SHUFFLE_FILTER,
+            self._SELECT_FIRST_N_FILTER,
+        ]
+
+    @property
     def _FILTER_CHAIN_WITH_REGION_AND_COUNTRY(self):
         return [
             self._UP_FILTER,
             self._COUNTRY_FILTER,
             self._REGION_FILTER,
             self._SELECT_FIRST_REGION_FILTER,
             self._PRIORITY_FILTER,
             self._WEIGHTED_SHUFFLE_FILTER,
             self._SELECT_FIRST_N_FILTER,
         ]
 
+    @property
+    def _FILTER_CHAIN_WITH_REGION_AND_SUBNET(self):
+        return [
+            self._UP_FILTER,
+            self._SUBNET_FILTER,
+            self._REGION_FILTER,
+            self._SELECT_FIRST_REGION_FILTER,
+            self._PRIORITY_FILTER,
+            self._WEIGHTED_SHUFFLE_FILTER,
+            self._SELECT_FIRST_N_FILTER,
+        ]
+
+    @property
+    def _FILTER_CHAIN_WITH_COUNTRY_AND_SUBNET(self):
+        return [
+            self._UP_FILTER,
+            self._SUBNET_FILTER,
+            self._COUNTRY_FILTER,
+            self._SELECT_FIRST_REGION_FILTER,
+            self._PRIORITY_FILTER,
+            self._WEIGHTED_SHUFFLE_FILTER,
+            self._SELECT_FIRST_N_FILTER,
+        ]
+
+    @property
+    def _FILTER_CHAIN_WITH_REGION_AND_COUNTRY_AND_SUBNET(self):
+        return [
+            self._UP_FILTER,
+            self._SUBNET_FILTER,
+            self._COUNTRY_FILTER,
+            self._REGION_FILTER,
+            self._SELECT_FIRST_REGION_FILTER,
+            self._PRIORITY_FILTER,
+            self._WEIGHTED_SHUFFLE_FILTER,
+            self._SELECT_FIRST_N_FILTER,
+        ]
+
     _REGION_TO_CONTINENT = {
         'AFRICA': 'AF',
         'ASIAPAC': 'AS',
         'EUROPE': 'EU',
         'SOUTH-AMERICA': 'SA',
         # continent NA has been handled as part of Geofence Country filter
         # starting from v0.9.13. These below US-* just need to continue to
@@ -414,35 +470,42 @@
     }
 
     def __init__(
         self,
         id,
         api_key,
         retry_count=4,
-        monitor_regions=None,
+        monitor_regions=[],
         parallelism=None,
         client_config=None,
         shared_notifylist=False,
+        use_http_monitors=False,
         default_healthcheck_http_version="HTTP/1.0",
         *args,
         **kwargs,
     ):
         self.log = getLogger(f'Ns1Provider[{id}]')
         self.log.debug(
             '__init__: id=%s, api_key=***, retry_count=%d, '
-            'monitor_regions=%s, parallelism=%s, client_config=%s',
+            'monitor_regions=%s, parallelism=%s, client_config=%s, '
+            'shared_notifylist=%s, use_http_monitors=%s, '
+            'default_healthcheck_http_version=%s',
             id,
             retry_count,
             monitor_regions,
             parallelism,
             client_config,
+            shared_notifylist,
+            use_http_monitors,
+            default_healthcheck_http_version,
         )
         super().__init__(id, *args, **kwargs)
         self.monitor_regions = monitor_regions
         self.shared_notifylist = shared_notifylist
+        self.use_http_monitors = use_http_monitors
         self.record_filters = dict()
         self._client = Ns1Client(
             api_key, parallelism, retry_count, client_config
         )
         self.default_healthcheck_http_version = default_healthcheck_http_version
 
     def _sanitize_disabled_in_filter_config(self, filter_cfg):
@@ -452,26 +515,35 @@
                 del filter['disabled']
         return filter_cfg
 
     def _valid_filter_config(self, filter_cfg):
         self._sanitize_disabled_in_filter_config(filter_cfg)
         has_region = self._REGION_FILTER in filter_cfg
         has_country = self._COUNTRY_FILTER in filter_cfg
+        has_subnet = self._SUBNET_FILTER in filter_cfg
         expected_filter_cfg = self._get_updated_filter_chain(
-            has_region, has_country
+            has_region, has_country, has_subnet
         )
         return filter_cfg == expected_filter_cfg
 
-    def _get_updated_filter_chain(self, has_region, has_country):
-        if has_region and has_country:
+    def _get_updated_filter_chain(self, has_region, has_country, has_subnet):
+        if has_region and has_country and has_subnet:
+            filter_chain = self._FILTER_CHAIN_WITH_REGION_AND_COUNTRY_AND_SUBNET
+        elif has_region and has_country:
             filter_chain = self._FILTER_CHAIN_WITH_REGION_AND_COUNTRY
+        elif has_region and has_subnet:
+            filter_chain = self._FILTER_CHAIN_WITH_REGION_AND_SUBNET
+        elif has_country and has_subnet:
+            filter_chain = self._FILTER_CHAIN_WITH_COUNTRY_AND_SUBNET
         elif has_region:
             filter_chain = self._FILTER_CHAIN_WITH_REGION
         elif has_country:
             filter_chain = self._FILTER_CHAIN_WITH_COUNTRY
+        elif has_subnet:
+            filter_chain = self._FILTER_CHAIN_WITH_SUBNET
         else:
             filter_chain = self._BASIC_FILTER_CHAIN
 
         return filter_chain
 
     def _encode_notes(self, data):
         return ' '.join([f'{k}:{v}' for k, v in sorted(data.items())])
@@ -526,17 +598,18 @@
         values = [str(x) for x in values]
         geo = OrderedDict({str(k): [str(x) for x in v] for k, v in geo.items()})
         data['values'] = values
         data['geo'] = geo
         return data
 
     def _parse_dynamic_pool_name(self, pool_name):
-        if pool_name.startswith('catchall__'):
+        catchall_prefix = 'catchall__'
+        if pool_name.startswith(catchall_prefix):
             # Special case for the old-style catchall prefix
-            return pool_name[10:]
+            return pool_name[len(catchall_prefix) :]
         try:
             pool_name, _ = pool_name.rsplit('__', 1)
         except ValueError:
             pass
         return pool_name
 
     def _parse_pools(self, answers):
@@ -683,14 +756,17 @@
                 rules[rule_order] = rule
 
             geos = self._parse_rule_geos(meta, notes)
             if geos:
                 # There are geos, combine them with any existing geos for this
                 # pool and recorded the sorted unique set of them
                 rule['geos'] = sorted(set(rule.get('geos', [])) | geos)
+            subnets = set(meta.get('ip_prefixes', []))
+            if subnets:
+                rule['subnets'] = sorted(subnets)
 
         # Convert to list and order
         rules = sorted(rules.values(), key=lambda r: (r['_order'], r['pool']))
 
         return rules
 
     def _data_for_dynamic(self, _type, record):
@@ -955,17 +1031,19 @@
                 data = self._parse_notes(monitor['notes'])
                 if not data:
                     continue
                 if (
                     expected_host == data['host']
                     and expected_type == data['type']
                 ):
-                    # This monitor does not belong to this record
-                    config = monitor['config']
-                    value = config['host']
+                    # This monitor belongs to this record
+                    value = data.get('value')
+                    if not value:
+                        # old style notes in TCP monitors
+                        value = monitor['config']['host']
                     if record._type == 'CNAME':
                         # Append a trailing dot for CNAME records so that
                         # lookup by a CNAME answer works
                         value = value + '.'
                     monitors[value] = monitor
 
         return monitors
@@ -1026,14 +1104,31 @@
         monitor['notify_list'] = nl['id']
         monitor = self._client.monitors_create(**monitor)
         monitor_id = monitor['id']
         self.log.debug('_monitor_create:   monitor=%s', monitor_id)
 
         return monitor_id, self._feed_create(monitor)
 
+    def _monitor_delete(self, monitor):
+        monitor_id = monitor['id']
+        feed_id = self._client.feeds_for_monitors.get(monitor_id)
+        if feed_id:
+            self._client.datafeed_delete(self._client.datasource_id, feed_id)
+
+        self._client.monitors_delete(monitor_id)
+
+        notify_list_id = monitor['notify_list']
+        for nl_name, nl in self._client.notifylists.items():
+            if nl['id'] == notify_list_id:
+                # We've found the that might need deleting
+                if nl['name'] != self.SHARED_NOTIFYLIST_NAME:
+                    # It's not shared so is safe to delete
+                    self._client.notifylists_delete(notify_list_id)
+                break
+
     def _healthcheck_policy(self, record):
         return (
             record._octodns.get('ns1', {})
             .get('healthcheck', {})
             .get('policy', 'quorum')
         )
 
@@ -1084,95 +1179,151 @@
 
         if _type == 'CNAME':
             # NS1 does not accept a host value with a trailing dot
             value = value[:-1]
 
         ret = {
             'active': True,
-            'config': {
-                'connect_timeout':
-                # TCP monitors use milliseconds, so convert from
-                # seconds to milliseconds
-                self._healthcheck_connect_timeout(record) * 1000,
-                'host': value,
-                'port': record.healthcheck_port,
-                'response_timeout':
-                # TCP monitors use milliseconds, so convert from
-                # seconds to milliseconds
-                self._healthcheck_response_timeout(record) * 1000,
-                'ssl': record.healthcheck_protocol == 'HTTPS',
-            },
-            'job_type': 'tcp',
             'name': f'{host} - {_type} - {value}',
-            'notes': self._encode_notes({'host': host, 'type': _type}),
+            'notes': {'host': host, 'type': _type},
             'policy': self._healthcheck_policy(record),
             'frequency': self._healthcheck_frequency(record),
             'rapid_recheck': self._healthcheck_rapid_recheck(record),
             'region_scope': 'fixed',
             'regions': self.monitor_regions,
         }
 
-        if _type == 'AAAA':
-            ret['config']['ipv6'] = True
+        connect_timeout = self._healthcheck_connect_timeout(record)
+        response_timeout = self._healthcheck_response_timeout(record)
+
+        if record.healthcheck_protocol == 'TCP' or not self.use_http_monitors:
+            ret['job_type'] = 'tcp'
+            ret['config'] = {
+                'host': value,
+                'port': record.healthcheck_port,
+                # TCP monitors use milliseconds, so convert from seconds to milliseconds
+                'connect_timeout': connect_timeout * 1000,
+                'response_timeout': response_timeout * 1000,
+                'ssl': record.healthcheck_protocol == 'HTTPS',
+            }
 
-        if record.healthcheck_protocol != 'TCP':
-            # IF it's HTTP we need to send the request string
+            if record.healthcheck_protocol != 'TCP':
+                # legacy HTTP-emulating TCP monitor
+                # we need to send the HTTP request string
+                path = record.healthcheck_path
+                host = record.healthcheck_host(value=value)
+                http_version = self._healthcheck_http_version(record)
+                request = (
+                    fr'GET {path} {http_version}\r\nHost: {host}\r\n'
+                    r'User-agent: NS1\r\n\r\n'
+                )
+                ret['config']['send'] = request
+                # We'll also expect a HTTP response
+                ret['rules'] = [
+                    {
+                        'comparison': 'contains',
+                        'key': 'output',
+                        'value': '200 OK',
+                    }
+                ]
+        else:
+            # modern HTTP monitor
+            ret['job_type'] = 'http'
+            proto = record.healthcheck_protocol.lower()
+            domain = f'[{value}]' if _type == 'AAAA' else value
+            port = record.healthcheck_port
             path = record.healthcheck_path
-            host = record.healthcheck_host(value=value)
-            http_version = self._healthcheck_http_version(record)
-            request = (
-                fr'GET {path} {http_version}\r\nHost: {host}\r\n'
-                r'User-agent: NS1\r\n\r\n'
-            )
-            ret['config']['send'] = request
-            # We'll also expect a HTTP response
+            ret['config'] = {
+                'url': f'{proto}://{domain}:{port}{path}',
+                'virtual_host': record.healthcheck_host(value=value),
+                'user_agent': 'NS1',
+                'tls_add_verify': False,
+                'follow_redirect': False,
+                'connect_timeout': connect_timeout,
+                'idle_timeout': response_timeout,
+            }
             ret['rules'] = [
-                {'comparison': 'contains', 'key': 'output', 'value': '200 OK'}
+                {'comparison': '==', 'key': 'status_code', 'value': '200'}
             ]
 
+        if _type == 'AAAA':
+            ret['config']['ipv6'] = True
+
+        if self.use_http_monitors:
+            ret['notes']['value'] = value
+        ret['notes'] = self._encode_notes(ret['notes'])
+
         return ret
 
     def _monitor_is_match(self, expected, have):
         # Make sure what we have matches what's in expected exactly. Anything
         # else in have will be ignored.
+        log_prefix = 'monitor mismatch'
+        if 'name' in have:
+            name = have['name']
+            log_prefix = f'monitor "{name}" mismatch'
         for k, v in expected.items():
             if k == 'config':
                 # config is a nested dict and we need to only consider keys in
                 # expected for it as well
                 have_config = have.get(k, {})
                 for k, v in v.items():
                     if have_config.get(k, '--missing--') != v:
+                        self.log.debug(
+                            f'{log_prefix}: got config.{k}={have_config.get(k)}, expected {v}'
+                        )
                         return False
+            elif k == 'regions':
+                # regions can be out of order
+                if set(have.get(k, [])) != set(v):
+                    self.log.info(
+                        f'{log_prefix}: got {k}={have.get(k)}, expected {v}'
+                    )
+                    return False
             elif have.get(k, '--missing--') != v:
+                self.log.info(
+                    f'{log_prefix}: got {k}={have.get(k)}, expected {v}'
+                )
                 return False
 
         return True
 
     def _monitor_sync(self, record, value, existing):
         self.log.debug('_monitor_sync: record=%s, value=%s', record.fqdn, value)
         expected = self._monitor_gen(record, value)
 
         if existing:
             self.log.debug('_monitor_sync:   existing=%s', existing['id'])
             monitor_id = existing['id']
+            feed_id = None
 
             if not self._monitor_is_match(expected, existing):
-                self.log.debug('_monitor_sync:   existing needs update')
-                # Update the monitor to match expected, everything else will be
-                # left alone and assumed correct
-                self._client.monitors_update(monitor_id, **expected)
+                if expected['job_type'] == existing['job_type']:
+                    self.log.debug('_monitor_sync:   existing needs update')
+                    # Update the monitor to match expected, everything else will be
+                    # left alone and assumed correct
+                    self._client.monitors_update(monitor_id, **expected)
+                else:
+                    # NS1 monitor job types cannot be changed, so we will do a
+                    # delete+create
+                    self.log.debug(
+                        '_monitor_sync: existing needs to be replaced (delete+create new)'
+                    )
+                    self._monitor_delete(existing)
+                    monitor_id, feed_id = self._monitor_create(expected)
 
-            feed_id = self._client.feeds_for_monitors.get(monitor_id)
-            if feed_id is None:
-                self.log.warning(
-                    '_monitor_sync: %s (%s) missing feed, creating',
-                    existing['name'],
-                    monitor_id,
-                )
-                feed_id = self._feed_create(existing)
+            if not feed_id:
+                feed_id = self._client.feeds_for_monitors.get(monitor_id)
+                if feed_id is None:
+                    self.log.warning(
+                        '_monitor_sync: %s (%s) missing feed, creating',
+                        existing['name'],
+                        monitor_id,
+                    )
+                    feed_id = self._feed_create(existing)
         else:
             self.log.debug('_monitor_sync:   needs create')
             # We don't have an existing monitor create it (and related bits)
             monitor_id, feed_id = self._monitor_create(expected)
 
         return monitor_id, feed_id
 
@@ -1189,30 +1340,15 @@
         for monitor in self._monitors_for(record).values():
             monitor_id = monitor['id']
             if monitor_id in active_monitor_ids:
                 continue
 
             self.log.debug('_monitors_gc:   deleting %s', monitor_id)
 
-            feed_id = self._client.feeds_for_monitors.get(monitor_id)
-            if feed_id:
-                self._client.datafeed_delete(
-                    self._client.datasource_id, feed_id
-                )
-
-            self._client.monitors_delete(monitor_id)
-
-            notify_list_id = monitor['notify_list']
-            for nl_name, nl in self._client.notifylists.items():
-                if nl['id'] == notify_list_id:
-                    # We've found the that might need deleting
-                    if nl['name'] != self.SHARED_NOTIFYLIST_NAME:
-                        # It's not shared so is safe to delete
-                        self._client.notifylists_delete(notify_list_id)
-                    break
+            self._monitor_delete(monitor)
 
     def _add_answers_for_pool(
         self,
         answers,
         default_answers,
         pool_name,
         pool_label,
@@ -1264,14 +1400,15 @@
                 },
                 'region': pool_label,  # the one we're answering
             }
             answers.append(answer)
 
     def _generate_regions(self, record):
         pools = record.dynamic.pools
+        has_subnet = False
         has_country = False
         has_region = False
         regions = {}
 
         explicit_countries = dict()
         for rule in record.dynamic.rules:
             for geo in rule.data.get('geos', []):
@@ -1288,14 +1425,15 @@
             if fallback:
                 notes['fallback'] = fallback
 
             country = set()
             georegion = set()
             us_state = set()
             ca_province = set()
+            subnet = set(rule.data.get('subnets', []))
 
             for geo in rule.data.get('geos', []):
                 n = len(geo)
                 if n == 8:
                     # US state, e.g. NA-US-KY
                     # CA province, e.g. NA-CA-NL
                     us_state.add(
@@ -1326,14 +1464,17 @@
                         country.update(continent_countries - exclude)
                         notes.setdefault('continents', set()).add(geo)
                         has_country = True
 
             if 'continents' in notes:
                 notes['continents'] = ','.join(sorted(notes['continents']))
 
+            if subnet:
+                has_subnet = True
+
             meta = {'note': self._encode_notes(notes)}
 
             if georegion:
                 georegion_meta = dict(meta)
                 georegion_meta['georegion'] = sorted(georegion)
                 regions[f'{pool_name}__georegion'] = {'meta': georegion_meta}
 
@@ -1347,19 +1488,25 @@
                 if country:
                     country_state_meta['country'] = sorted(country)
                 if us_state:
                     country_state_meta['us_state'] = sorted(us_state)
                 if ca_province:
                     country_state_meta['ca_province'] = sorted(ca_province)
                 regions[f'{pool_name}__country'] = {'meta': country_state_meta}
-            elif not georegion:
+
+            if subnet:
+                subnet_meta = dict(meta)
+                subnet_meta['ip_prefixes'] = sorted(subnet)
+                regions[f'{pool_name}__subnet'] = {'meta': subnet_meta}
+
+            if not (subnet or country or us_state or ca_province or georegion):
                 # If there's no targeting it's a catchall
                 regions[f'{pool_name}__catchall'] = {'meta': meta}
 
-        return has_country, has_region, regions
+        return has_subnet, has_country, has_region, regions
 
     def _generate_answers(self, record, regions):
         pools = record.dynamic.pools
         existing_monitors = self._monitors_for(record)
         active_monitors = set()
 
         # Build a list of primary values for each pool, including their
@@ -1401,42 +1548,44 @@
             default_values = record.values
         default_answers = [{'answer': [v], 'weight': 1} for v in default_values]
 
         # Build our list of answers
         # The regions dictionary built above already has the required pool
         # names. Iterate over them and add answers.
         answers = []
-        for pool_name in sorted(regions.keys()):
+        for pool_label in sorted(regions.keys()):
             priority = 1
 
-            # Dynamic/health checked
-            pool_label = pool_name
             # Remove the pool type from the end of the name
-            pool_name = self._parse_dynamic_pool_name(pool_name)
+            pool_name = self._parse_dynamic_pool_name(pool_label)
             self._add_answers_for_pool(
                 answers,
                 default_answers,
                 pool_name,
                 pool_label,
                 pool_answers,
                 pools,
                 priority,
             )
 
         return active_monitors, answers
 
     def _params_for_dynamic(self, record):
         # Convert rules to regions
-        has_country, has_region, regions = self._generate_regions(record)
+        has_subnet, has_country, has_region, regions = self._generate_regions(
+            record
+        )
 
         # Convert pools to answers
         active_monitors, answers = self._generate_answers(record, regions)
 
         # Update filters as necessary
-        filters = self._get_updated_filter_chain(has_region, has_country)
+        filters = self._get_updated_filter_chain(
+            has_region, has_country, has_subnet
+        )
 
         return {
             'answers': answers,
             'filters': filters,
             'regions': regions,
             'ttl': record.ttl,
         }, active_monitors
@@ -1511,18 +1660,20 @@
         return {'answers': values, 'ttl': record.ttl}, None
 
     def _extra_changes(self, desired, changes, **kwargs):
         self.log.debug('_extra_changes: desired=%s', desired.name)
         changed = set([c.record for c in changes])
         extra = []
         for record in desired.records:
-            if record in changed or not getattr(record, 'dynamic', False):
-                # Already changed, or no dynamic , no need to check it
+            if not getattr(record, 'dynamic', False):
+                # no need to check non-dynamic simple records
                 continue
 
+            update = False
+
             # Filter normalization
             # Check if filters for existing domains need an update
             # Needs an explicit check since there might be no change in the
             # config at all. Filters however might still need an update
             domain = record.fqdn[:-1]
             _type = record._type
             record_filters = self.record_filters.get(domain, {}).get(_type, [])
@@ -1530,36 +1681,73 @@
                 # unrecognized set of filters, overwrite them by updating the
                 # record
                 self.log.info(
                     '_extra_changes: unrecognized filters in %s, '
                     'will update record',
                     domain,
                 )
-                extra.append(Update(record, record))
-                continue
+                update = True
 
-            for value, have in self._monitors_for(record).items():
-                expected = self._monitor_gen(record, value)
-                # TODO: find values which have missing monitors
-                if not self._monitor_is_match(expected, have):
-                    self.log.info(
-                        '_extra_changes: monitor mis-match for %s',
-                        expected['name'],
-                    )
-                    extra.append(Update(record, record))
-                    break
-                if not have.get('notify_list'):
-                    self.log.info(
-                        '_extra_changes: broken monitor no notify '
-                        'list %s (%s)',
-                        have['name'],
-                        have['id'],
-                    )
-                    extra.append(Update(record, record))
-                    break
+            # check if any monitor needs to be synced
+            existing = self._monitors_for(record)
+            for pool in record.dynamic.pools.values():
+                for val in pool.data['values']:
+                    if val['status'] != 'obey':
+                        # no monitor necessary
+                        continue
+
+                    value = val['value']
+                    expected = self._monitor_gen(record, value)
+                    name = expected['name']
+
+                    have = existing.get(value)
+                    if not have:
+                        if self.use_http_monitors:
+                            self.log.warning(
+                                '_extra_changes: missing monitor "%s" will be created of type http, '
+                                'octodns-ns1 cannot be downgraded below v0.0.5 after applying this change',
+                                name,
+                            )
+                        else:
+                            self.log.info(
+                                '_extra_changes: missing monitor %s', name
+                            )
+                        update = True
+                        continue
+
+                    if not self._monitor_is_match(expected, have):
+                        if expected['job_type'] == have['job_type']:
+                            self.log.info(
+                                '_extra_changes: monitor mis-match for %s', name
+                            )
+                        else:
+                            # NS1 monitor job types cannot be changed, so we need to do
+                            # delete+create, which has a few implications:
+                            self.log.warning(
+                                '_extra_changes: existing %s monitor "%s" will be deleted and replaced by a new %s monitor, '
+                                '`%s` will be temporarily treated as being healthy as a result, '
+                                'this is operation will be irreversible and not forward-compatible, ie '
+                                'octodns-ns1 cannot be downgraded below v0.0.5 after applying this change',
+                                have['job_type'],
+                                name,
+                                expected['job_type'],
+                                value,
+                            )
+                        update = True
+
+                    if not have.get('notify_list'):
+                        self.log.info(
+                            '_extra_changes: broken monitor no notify list %s (%s)',
+                            name,
+                            have['id'],
+                        )
+                        update = True
+
+            if update and record not in changed:
+                extra.append(Update(record, record))
 
         return extra
 
     def _apply_Create(self, ns1_zone, change):
         new = change.new
         zone = new.zone.name[:-1]
         domain = new.fqdn[:-1]
@@ -1600,15 +1788,15 @@
         self.log.debug(
             '_apply: zone=%s, len(changes)=%d', desired.name, len(changes)
         )
 
         # Make sure that if we're going to make any dynamic changes that we
         # have monitor_regions configured before touching anything so we can
         # abort early and not half-apply
-        if self._has_dynamic(changes) and self.monitor_regions is None:
+        if self._has_dynamic(changes) and not self.monitor_regions:
             raise Ns1Exception('Monitored record, but monitor_regions not set')
 
         domain_name = desired.name[:-1]
         try:
             ns1_zone = self._client.zones_retrieve(domain_name)
         except ResourceException as e:
             if e.message != self.ZONE_NOT_FOUND_MESSAGE:
```

### Comparing `octodns-ns1-0.0.4/octodns_ns1.egg-info/PKG-INFO` & `octodns-ns1-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: octodns-ns1
-Version: 0.0.4
-Summary:  NS1 provider for octoDNS
-Home-page: https://github.com/octodns/octodns-ns1
-Author: Ross McFarland
-Author-email: rwmcfa1@gmail.com
-License: MIT
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-
 ## NS1 provider for octoDNS
 
 An [octoDNS](https://github.com/octodns/octodns/) provider that targets [NS1](https://ns1.com/products/managed-dns).
 
 ### Installation
 
 #### Command line
@@ -70,17 +57,22 @@
     retry_count: 4
     # Optional. Default: None. Additional options or overrides passed to
     # the NS1 SDK config, as key-value pairs.
     client_config:
         endpoint: my.nsone.endpoint # Default: api.nsone.net
         ignore-ssl-errors: true     # Default: false
         follow_pagination: false    # Default: true
-    # Optional. Default: HTTP/1.0 . Default HTTP protocol to use when 
-    # health-checking dynamic record endpoints. See "Health Check Options" 
+    # Optional. Default: false. Use modern HTTP monitor (true) or the legacy
+    # HTTP-emulating TCP monitor (false) for HTTP(s) healthchecks.
+    use_http_monitors: false
+    # Optional. Default: HTTP/1.0. Default HTTP protocol to use when
+    # health-checking dynamic record endpoints. See "Health Check Options"
     # README section below to override per dynamic record.
+    # This is only supported when use_http_monitors is set to false. If it
+    # is set to true, HTTP/1.1 will be used and it cannot be changed.
     default_healthcheck_http_version: HTTP/1.0
 
 ```
 
 ### Support Information
 
 #### Records
@@ -91,26 +83,30 @@
 
 Ns1Provider supports full root NS record management.
 
 #### Dynamic
 
 Ns1Provider supports dynamic records.
 
+#### Subnet targeting
+
+Ns1Provider supports [subnet targeting](https://github.com/octodns/octodns/blob/main/docs/dynamic_records.md#subnets) in dynamic records.
+
 #### Health Check Options
 
 See https://github.com/octodns/octodns/blob/master/docs/dynamic_records.md#health-checks for information on health checking for dynamic records. Ns1Provider supports the following options:
 
 | Key  | Description | Default |
 |--|--|--|
 | policy | One of:<ol><li>`all` - down if every region is down</li><li>`quorum` - down if majority regions are down</li><li>`one` - down if any region is down</ol> | `quorum` |
 | frequency | Frequency (in seconds) of health-check | 60 |
 | connect_timeout | Timeout (in seconds) before we give up trying to connect | 2 |
 | response_timeout | Timeout (in seconds) after connecting to wait for output | 10 |
 | rapid_recheck | Enable or disable a second, automatic verification test before changing the status of a host. Enabling this option can help prevent false positives. | False |
-| http_version | Specify HTTP version to use when HTTP health-checking  a host. One of <ol><li>`HTTP/1.0`</li><li>`HTTP/1.1`</li><ol> | `HTTP/1.0` |
+| http_version | Specify HTTP version to use when HTTP health-checking a host. Only applicable if `use_http_monitors=False`. One of <ol><li>`HTTP/1.0`</li><li>`HTTP/1.1`</li><ol> | `HTTP/1.0` |
 
 ```yaml
 ---
   octodns:
     ns1:
       healthcheck:
         policy: quorum
```

### Comparing `octodns-ns1-0.0.4/setup.py` & `octodns-ns1-0.0.5/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -38,32 +38,36 @@
 setup(
     author='Ross McFarland',
     author_email='rwmcfa1@gmail.com',
     description=description,
     extras_require={
         'dev': tests_require
         + (
-            'black>=22.3.0',
+            # we need to manually/explicitely bump major versions as they're
+            # likely to result in formatting changes that should happen in their
+            # own PR. This will basically happen yearly
+            # https://black.readthedocs.io/en/stable/the_black_code_style/index.html#stability-policy
+            'black>=23.1.0,<24.0.0',
             'build>=0.7.0',
-            'isort>=5.11.4',
+            'isort>=5.11.5',
             'pyflakes>=2.2.0',
             'readme_renderer[md]>=26.0',
             'twine>=3.4.2',
         ),
         'test': tests_require,
     },
     install_requires=(
-        'octodns>=0.9.16',
+        'octodns>=1.0.0rc0',
         'ns1_python>=0.17.1',
         'pycountry-convert>=0.7.2',
         'requests>=2.27.1',
     ),
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     name='octodns-ns1',
     packages=find_packages(),
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     tests_require=tests_require,
     url='https://github.com/octodns/octodns-ns1',
     version=version(),
 )
```

### Comparing `octodns-ns1-0.0.4/tests/test_provider_ns1.py` & `octodns-ns1-0.0.5/tests/test_provider_ns1.py`

 * *Files 7% similar despite different names*

```diff
@@ -895,14 +895,18 @@
             'config': {'host': '2.3.4.5'},
             'notes': 'host:unit.tests type:A',
         }
         monitor_five = {
             'config': {'host': 'iad.unit.tests'},
             'notes': 'host:foo.unit.tests type:CNAME',
         }
+        monitor_eight = {
+            'config': {'url': 'https://iad.unit.tests/_ping'},
+            'notes': 'host:foo.unit.tests type:CNAME value:iad.unit.tests',
+        }
         provider._client._monitors_cache = {
             'one': monitor_one,
             'two': {
                 'config': {'host': '8.8.8.8'},
                 'notes': 'host:unit.tests type:AAAA',
             },
             'three': {
@@ -934,14 +938,21 @@
 
         # Check match for CNAME values
         self.assertEqual(
             {'iad.unit.tests.': monitor_five},
             provider._monitors_for(self.cname_record()),
         )
 
+        # Check for HTTP monitors match from notes
+        provider._client._monitors_cache['eight'] = monitor_eight
+        self.assertEqual(
+            {'iad.unit.tests.': monitor_eight},
+            provider._monitors_for(self.cname_record()),
+        )
+
     def test_uuid(self):
         # Just a smoke test/for coverage
         provider = Ns1Provider('test', 'api-key')
         self.assertTrue(provider._uuid())
 
     @patch('octodns_ns1.Ns1Provider._uuid')
     @patch('ns1.rest.data.Feed.create')
@@ -1051,29 +1062,40 @@
 
     def test_monitor_gen(self):
         provider = Ns1Provider('test', 'api-key')
 
         value = '3.4.5.6'
         record = self.record()
         monitor = provider._monitor_gen(record, value)
+        self.assertEqual('tcp', monitor['job_type'])
         self.assertEqual(value, monitor['config']['host'])
         self.assertTrue('\\nHost: send.me\\r' in monitor['config']['send'])
         self.assertFalse(monitor['config']['ssl'])
         self.assertEqual('host:unit.tests type:A', monitor['notes'])
 
         record._octodns['healthcheck']['host'] = None
         monitor = provider._monitor_gen(record, value)
         self.assertTrue(r'\nHost: 3.4.5.6\r' in monitor['config']['send'])
 
+        # Test http version validation
+        record._octodns['ns1']['healthcheck']['http_version'] = 'invalid'
+        with self.assertRaisesRegex(
+            Ns1Exception,
+            r"unsupported http version found: 'invalid'. Expected version in \('HTTP/1.0', 'HTTP/1.1'\)",
+        ):
+            provider._monitor_gen(record, value)
+        record._octodns['ns1']['healthcheck']['http_version'] = 'HTTP/1.0'
+
         record._octodns['healthcheck']['protocol'] = 'HTTPS'
         monitor = provider._monitor_gen(record, value)
         self.assertTrue(monitor['config']['ssl'])
 
         record._octodns['healthcheck']['protocol'] = 'TCP'
         monitor = provider._monitor_gen(record, value)
+        self.assertEqual('tcp', monitor['job_type'])
         # No http send done
         self.assertFalse('send' in monitor['config'])
         # No http response expected
         self.assertFalse('rules' in monitor)
 
         record._octodns['ns1']['healthcheck']['policy'] = 'all'
         monitor = provider._monitor_gen(record, value)
@@ -1091,38 +1113,80 @@
         monitor = provider._monitor_gen(record, value)
         self.assertEqual(1000, monitor['config']['connect_timeout'])
 
         record._octodns['ns1']['healthcheck']['response_timeout'] = 2
         monitor = provider._monitor_gen(record, value)
         self.assertEqual(2000, monitor['config']['response_timeout'])
 
-        # Test http version validation
+    def test_monitor_gen_http(self):
+        provider = Ns1Provider('test', 'api-key', use_http_monitors=True)
+
+        value = '3.4.5.6'
+        record = self.record()
+        monitor = provider._monitor_gen(record, value)
+        self.assertEqual('http', monitor['job_type'])
+        self.assertEqual(f'http://{value}:80/_ping', monitor['config']['url'])
+        self.assertEqual('send.me', monitor['config']['virtual_host'])
+        self.assertEqual(
+            f'host:unit.tests type:A value:{value}', monitor['notes']
+        )
+
+        record._octodns['healthcheck']['host'] = None
+        monitor = provider._monitor_gen(record, value)
+        self.assertEqual(value, monitor['config']['virtual_host'])
+
+        record._octodns['healthcheck']['protocol'] = 'HTTPS'
+        monitor = provider._monitor_gen(record, value)
+        self.assertTrue(monitor['config']['url'].startswith('https://'))
+
+        # http version doesn't matter or fail
         record._octodns['ns1']['healthcheck']['http_version'] = 'invalid'
-        with self.assertRaisesRegex(
-            Ns1Exception,
-            r"unsupported http version found: 'invalid'. Expected version in \('HTTP/1.0', 'HTTP/1.1'\)",
-        ):
-            provider._healthcheck_http_version(record)
+        provider._monitor_gen(record, value)
         record._octodns['ns1']['healthcheck']['http_version'] = 'HTTP/1.0'
 
-    def test_monitor_gen_AAAA(self):
-        provider = Ns1Provider('test', 'api-key')
+        record._octodns['ns1']['healthcheck']['connect_timeout'] = 1
+        monitor = provider._monitor_gen(record, value)
+        self.assertEqual(1, monitor['config']['connect_timeout'])
+
+        record._octodns['ns1']['healthcheck']['response_timeout'] = 2
+        monitor = provider._monitor_gen(record, value)
+        self.assertEqual(2, monitor['config']['idle_timeout'])
+
+        record._octodns['healthcheck']['protocol'] = 'TCP'
+        monitor = provider._monitor_gen(record, value)
+        self.assertEqual('tcp', monitor['job_type'])
+        # Nothing to send
+        self.assertFalse('send' in monitor['config'])
+        # Nothing to expect
+        self.assertFalse('rules' in monitor)
+
+        record._octodns['ns1']['healthcheck']['connect_timeout'] = 1
+        monitor = provider._monitor_gen(record, value)
+        self.assertEqual(1000, monitor['config']['connect_timeout'])
+
+        record._octodns['ns1']['healthcheck']['response_timeout'] = 2
+        monitor = provider._monitor_gen(record, value)
+        self.assertEqual(2000, monitor['config']['response_timeout'])
+
+    def test_monitor_gen_AAAA_http(self):
+        provider = Ns1Provider('test', 'api-key', use_http_monitors=True)
 
         value = '::ffff:3.4.5.6'
         record = self.aaaa_record()
         monitor = provider._monitor_gen(record, value)
         self.assertTrue(monitor['config']['ipv6'])
+        self.assertTrue(f'[{value}]' in monitor['config']['url'])
 
-    def test_monitor_gen_CNAME(self):
-        provider = Ns1Provider('test', 'api-key')
+    def test_monitor_gen_CNAME_http(self):
+        provider = Ns1Provider('test', 'api-key', use_http_monitors=True)
 
         value = 'iad.unit.tests.'
         record = self.cname_record()
         monitor = provider._monitor_gen(record, value)
-        self.assertEqual(value[:-1], monitor['config']['host'])
+        self.assertTrue(value[:-1] in monitor['config']['url'])
 
     def test_monitor_is_match(self):
         provider = Ns1Provider('test', 'api-key')
 
         # Empty matches empty
         self.assertTrue(provider._monitor_is_match({}, {}))
 
@@ -1156,23 +1220,37 @@
         self.assertTrue(
             provider._monitor_is_match(
                 {'config': {'key': 42, 'value': 43}},
                 {'config': {'key': 42, 'value': 43, 'other': 44}},
             )
         )
 
+        # missing regions causes mismatch
+        self.assertFalse(
+            provider._monitor_is_match({'regions': ['lga', 'sin']}, {})
+        )
+
+        # out of order regions doesn't cause mismatch
+        self.assertTrue(
+            provider._monitor_is_match(
+                {'regions': ['lga', 'sin']}, {'regions': ['sin', 'lga']}
+            )
+        )
+
     @patch('octodns_ns1.Ns1Provider._feed_create')
+    @patch('octodns_ns1.Ns1Provider._monitor_delete')
     @patch('octodns_ns1.Ns1Client.monitors_update')
     @patch('octodns_ns1.Ns1Provider._monitor_create')
     @patch('octodns_ns1.Ns1Provider._monitor_gen')
     def test_monitor_sync(
         self,
         monitor_gen_mock,
         monitor_create_mock,
         monitors_update_mock,
+        monitor_delete_mock,
         feed_create_mock,
     ):
         provider = Ns1Provider('test', 'api-key')
 
         # pre-fill caches to avoid extranious calls (things we're testing
         # elsewhere)
         provider._client._datasource_id = 'foo'
@@ -1219,25 +1297,42 @@
         self.assertEqual('mon-id2', monitor_id)
         self.assertEqual('feed-id2', feed_id)
         monitor_gen_mock.assert_called_once()
         monitor_create_mock.assert_not_called()
         monitors_update_mock.assert_not_called()
         feed_create_mock.assert_has_calls([call(monitor)])
 
-        # Existing monitor that needs updates
+        # Existing monitor of same job_type that needs updates
         reset()
-        monitor = {'id': 'mon-id', 'key': 'value', 'name': 'monitor name'}
-        gened = {'other': 'thing'}
+        monitor = {'id': 'mon-id', 'job_type': 'value', 'name': 'monitor name'}
+        gened = {'other': 'thing', 'job_type': 'value'}
         monitor_gen_mock.side_effect = [gened]
         monitor_id, feed_id = provider._monitor_sync(record, value, monitor)
         self.assertEqual('mon-id', monitor_id)
         self.assertEqual('feed-id', feed_id)
         monitor_gen_mock.assert_called_once()
         monitor_create_mock.assert_not_called()
-        monitors_update_mock.assert_has_calls([call('mon-id', other='thing')])
+        monitors_update_mock.assert_has_calls(
+            [call('mon-id', other='thing', job_type='value')]
+        )
+        feed_create_mock.assert_not_called()
+
+        # Existing monitor of different job_type that needs updates
+        reset()
+        monitor = {'id': 'mon-id', 'job_type': 'value', 'name': 'monitor name'}
+        gened = {'other': 'thing', 'job_type': 'value2'}
+        monitor_gen_mock.side_effect = [gened]
+        monitor_create_mock.side_effect = [('mon-id3', 'feed-id3')]
+        monitor_id, feed_id = provider._monitor_sync(record, value, monitor)
+        self.assertEqual('mon-id3', monitor_id)
+        self.assertEqual('feed-id3', feed_id)
+        monitor_gen_mock.assert_called_once()
+        monitor_delete_mock.assert_has_calls([call(monitor)])
+        monitor_create_mock.assert_has_calls([call(gened)])
+        monitors_update_mock.assert_not_called()
         feed_create_mock.assert_not_called()
 
     @patch('octodns_ns1.Ns1Client.notifylists_delete')
     @patch('octodns_ns1.Ns1Client.monitors_delete')
     @patch('octodns_ns1.Ns1Client.datafeed_delete')
     @patch('octodns_ns1.Ns1Provider._monitors_for')
     def test_monitors_gc(
@@ -1480,14 +1575,66 @@
                         'note': 'fallback:iad rule-order:0',
                     }
                 },
             },
             ret['regions'],
         )
 
+    @patch('octodns_ns1.Ns1Provider._monitors_for')
+    def test_params_for_dynamic_subnet_only(self, monitors_for_mock):
+        provider = Ns1Provider('test', 'api-key')
+
+        # provider._params_for_A() calls provider._monitors_for().
+        # Mock it's return value so that we don't make NS1 API calls during tests
+        monitors_for_mock.reset_mock()
+        monitors_for_mock.side_effect = [{}]
+
+        dynamic_rules = [
+            {'subnets': ['10.1.0.0/16'], 'pool': 'lhr'},
+            {'pool': 'iad'},
+        ]
+        record = Record.new(
+            self.zone,
+            '',
+            {
+                'dynamic': {
+                    'pools': {
+                        'lhr': {
+                            'values': [{'value': '3.4.5.6', 'status': 'up'}]
+                        },
+                        'iad': {
+                            'values': [{'value': '5.6.7.8', 'status': 'up'}]
+                        },
+                    },
+                    'rules': dynamic_rules,
+                },
+                'ttl': 32,
+                'type': 'A',
+                'value': '1.2.3.4',
+                'meta': {},
+            },
+        )
+        ret, _ = provider._params_for_A(record)
+        self.assertEqual(4, len(ret['answers']))
+        exp = provider._FILTER_CHAIN_WITH_SUBNET
+        self.assertEqual(ret['filters'], exp)
+        exp_regions = {
+            'iad__catchall': {'meta': {'note': 'rule-order:1'}},
+            'lhr__subnet': {
+                'meta': {'ip_prefixes': ['10.1.0.0/16'], 'note': 'rule-order:0'}
+            },
+        }
+        self.assertEqual(exp_regions, ret['regions'])
+
+        # test parsing back into the same dynamic rules
+        parsed_rules = provider._parse_rules({}, exp_regions)
+        for rule in parsed_rules:
+            del rule['_order']
+        self.assertEqual(dynamic_rules, parsed_rules)
+
     @patch('octodns_ns1.Ns1Provider._monitor_sync')
     @patch('octodns_ns1.Ns1Provider._monitors_for')
     def test_params_for_dynamic_contient_and_countries(
         self, monitors_for_mock, monitor_sync_mock
     ):
         provider = Ns1Provider('test', 'api-key')
 
@@ -1595,14 +1742,188 @@
                         'note': 'fallback:iad rule-order:0',
                     }
                 },
             },
             ret['regions'],
         )
 
+    @patch('octodns_ns1.Ns1Provider._monitors_for')
+    def test_params_for_dynamic_region_and_subnet(self, monitors_for_mock):
+        provider = Ns1Provider('test', 'api-key')
+
+        # provider._params_for_A() calls provider._monitors_for().
+        # Mock it's return value so that we don't make NS1 API calls during tests
+        monitors_for_mock.reset_mock()
+        monitors_for_mock.side_effect = [{}]
+
+        dynamic_rules = [
+            {'subnets': ['10.1.0.0/16'], 'geos': ['EU'], 'pool': 'lhr'},
+            {'pool': 'iad'},
+        ]
+        record = Record.new(
+            self.zone,
+            '',
+            {
+                'dynamic': {
+                    'pools': {
+                        'lhr': {
+                            'values': [{'value': '3.4.5.6', 'status': 'up'}]
+                        },
+                        'iad': {
+                            'values': [{'value': '5.6.7.8', 'status': 'up'}]
+                        },
+                    },
+                    'rules': dynamic_rules,
+                },
+                'ttl': 32,
+                'type': 'A',
+                'value': '1.2.3.4',
+                'meta': {},
+            },
+        )
+        ret, _ = provider._params_for_A(record)
+        self.assertEqual(6, len(ret['answers']))
+        exp = provider._FILTER_CHAIN_WITH_REGION_AND_SUBNET
+        self.assertEqual(ret['filters'], exp)
+        exp_regions = {
+            'iad__catchall': {'meta': {'note': 'rule-order:1'}},
+            'lhr__subnet': {
+                'meta': {'ip_prefixes': ['10.1.0.0/16'], 'note': 'rule-order:0'}
+            },
+            'lhr__georegion': {
+                'meta': {'georegion': ['EUROPE'], 'note': 'rule-order:0'}
+            },
+        }
+        self.assertEqual(exp_regions, ret['regions'])
+
+        # test parsing back into the same dynamic rules
+        parsed_rules = provider._parse_rules({}, exp_regions)
+        for rule in parsed_rules:
+            del rule['_order']
+        self.assertEqual(dynamic_rules, parsed_rules)
+
+    @patch('octodns_ns1.Ns1Provider._monitors_for')
+    def test_params_for_dynamic_country_and_subnet(self, monitors_for_mock):
+        provider = Ns1Provider('test', 'api-key')
+
+        # provider._params_for_A() calls provider._monitors_for().
+        # Mock it's return value so that we don't make NS1 API calls during tests
+        monitors_for_mock.reset_mock()
+        monitors_for_mock.side_effect = [{}]
+
+        dynamic_rules = [
+            {'subnets': ['10.1.0.0/16'], 'geos': ['EU-GB'], 'pool': 'lhr'},
+            {'pool': 'iad'},
+        ]
+        record = Record.new(
+            self.zone,
+            '',
+            {
+                'dynamic': {
+                    'pools': {
+                        'lhr': {
+                            'values': [{'value': '3.4.5.6', 'status': 'up'}]
+                        },
+                        'iad': {
+                            'values': [{'value': '5.6.7.8', 'status': 'up'}]
+                        },
+                    },
+                    'rules': dynamic_rules,
+                },
+                'ttl': 32,
+                'type': 'A',
+                'value': '1.2.3.4',
+                'meta': {},
+            },
+        )
+        ret, _ = provider._params_for_A(record)
+        self.assertEqual(6, len(ret['answers']))
+        exp = provider._FILTER_CHAIN_WITH_COUNTRY_AND_SUBNET
+        self.assertEqual(ret['filters'], exp)
+        exp_regions = {
+            'iad__catchall': {'meta': {'note': 'rule-order:1'}},
+            'lhr__subnet': {
+                'meta': {'ip_prefixes': ['10.1.0.0/16'], 'note': 'rule-order:0'}
+            },
+            'lhr__country': {
+                'meta': {'country': ['GB'], 'note': 'rule-order:0'}
+            },
+        }
+        self.assertEqual(exp_regions, ret['regions'])
+
+        # test parsing back into the same dynamic rules
+        parsed_rules = provider._parse_rules({}, exp_regions)
+        for rule in parsed_rules:
+            del rule['_order']
+        self.assertEqual(dynamic_rules, parsed_rules)
+
+    @patch('octodns_ns1.Ns1Provider._monitors_for')
+    def test_params_for_dynamic_region_and_country_and_subnet(
+        self, monitors_for_mock
+    ):
+        provider = Ns1Provider('test', 'api-key')
+
+        # provider._params_for_A() calls provider._monitors_for().
+        # Mock it's return value so that we don't make NS1 API calls during tests
+        monitors_for_mock.reset_mock()
+        monitors_for_mock.side_effect = [{}]
+
+        dynamic_rules = [
+            {
+                'subnets': ['10.1.0.0/16'],
+                'geos': ['AF', 'EU-GB'],
+                'pool': 'lhr',
+            },
+            {'pool': 'iad'},
+        ]
+        record = Record.new(
+            self.zone,
+            '',
+            {
+                'dynamic': {
+                    'pools': {
+                        'lhr': {
+                            'values': [{'value': '3.4.5.6', 'status': 'up'}]
+                        },
+                        'iad': {
+                            'values': [{'value': '5.6.7.8', 'status': 'up'}]
+                        },
+                    },
+                    'rules': dynamic_rules,
+                },
+                'ttl': 32,
+                'type': 'A',
+                'value': '1.2.3.4',
+                'meta': {},
+            },
+        )
+        ret, _ = provider._params_for_A(record)
+        self.assertEqual(8, len(ret['answers']))
+        exp = provider._FILTER_CHAIN_WITH_REGION_AND_COUNTRY_AND_SUBNET
+        self.assertEqual(ret['filters'], exp)
+        exp_regions = {
+            'iad__catchall': {'meta': {'note': 'rule-order:1'}},
+            'lhr__subnet': {
+                'meta': {'ip_prefixes': ['10.1.0.0/16'], 'note': 'rule-order:0'}
+            },
+            'lhr__country': {
+                'meta': {'country': ['GB'], 'note': 'rule-order:0'}
+            },
+            'lhr__georegion': {
+                'meta': {'georegion': ['AFRICA'], 'note': 'rule-order:0'}
+            },
+        }
+        self.assertEqual(exp_regions, ret['regions'])
+
+        # test parsing back into the same dynamic rules
+        parsed_rules = provider._parse_rules({}, exp_regions)
+        for rule in parsed_rules:
+            del rule['_order']
+        self.assertEqual(dynamic_rules, parsed_rules)
+
     @patch('octodns_ns1.Ns1Provider._monitor_sync')
     @patch('octodns_ns1.Ns1Provider._monitors_for')
     def test_params_for_dynamic_oceania(
         self, monitors_for_mock, monitor_sync_mock
     ):
         provider = Ns1Provider('test', 'api-key')
 
@@ -1742,15 +2063,15 @@
                 'values': [],
             },
             data,
         )
 
         # Test out a small, but realistic setup that covers all the options
         # We have country and region in the test config
-        filters = provider._get_updated_filter_chain(True, True)
+        filters = provider._get_updated_filter_chain(True, True, False)
         catchall_pool_name = 'iad__catchall'
         ns1_record = {
             'answers': [
                 {
                     'answer': ['3.4.5.6'],
                     'meta': {
                         'priority': 1,
@@ -2047,15 +2368,15 @@
     def test_data_for_dynamic_CNAME(self):
         provider = Ns1Provider('test', 'api-key')
 
         # Test out a small setup that just covers default value validation
         # Everything else is same as dynamic A whose tests will cover all
         # other options and test cases
         # Not testing for geo/region specific cases
-        filters = provider._get_updated_filter_chain(False, False)
+        filters = provider._get_updated_filter_chain(False, False, False)
         catchall_pool_name = 'iad__catchall'
         ns1_record = {
             'answers': [
                 {
                     'answer': ['iad.unit.tests.'],
                     'meta': {
                         'priority': 1,
@@ -2104,15 +2425,15 @@
         )
 
     def test_data_for_invalid_dynamic_CNAME(self):
         provider = Ns1Provider('test', 'api-key')
 
         # Potential setup created outside of octoDNS, so it could be missing
         # notes and region names can be arbitrary
-        filters = provider._get_updated_filter_chain(False, False)
+        filters = provider._get_updated_filter_chain(False, False, False)
         ns1_record = {
             'answers': [
                 {
                     'answer': ['iad.unit.tests.'],
                     'meta': {'priority': 1, 'weight': 12, 'up': {}},
                     'region': 'global',
                 },
@@ -2245,15 +2566,17 @@
         )
         desired.add_record(dynamic)
 
         # untouched, but everything in sync so no change needed
         reset()
         # Generate what we expect to have
         provider.record_filters[dynamic.fqdn[:-1]] = {
-            dynamic._type: provider._get_updated_filter_chain(False, False)
+            dynamic._type: provider._get_updated_filter_chain(
+                False, False, False
+            )
         }
         gend = provider._monitor_gen(dynamic, '1.2.3.4')
         gend.update(
             {
                 'id': 'mid',  # need to add an id
                 'notify_list': 'xyz',  # need to add a notify list (for now)
             }
@@ -2272,34 +2595,61 @@
         monitors_for_mock.side_effect = [{'1.2.3.4': gend}]
         extra = provider._extra_changes(desired, [])
         self.assertEqual(1, len(extra))
         extra = list(extra)[0]
         self.assertIsInstance(extra, Update)
         self.assertEqual(dynamic, extra.new)
         monitors_for_mock.assert_has_calls([call(dynamic)])
+        gend['notify_list'] = 'xyz'
 
-        # Add notify_list back and change the healthcheck protocol, we'll still
+        # change the healthcheck protocol, we'll still
         # expect to see an update
         reset()
-        gend['notify_list'] = 'xyz'
         dynamic._octodns['healthcheck']['protocol'] = 'HTTPS'
-        del gend['notify_list']
         monitors_for_mock.side_effect = [{'1.2.3.4': gend}]
         extra = provider._extra_changes(desired, [])
         self.assertEqual(1, len(extra))
         extra = list(extra)[0]
         self.assertIsInstance(extra, Update)
         self.assertEqual(dynamic, extra.new)
         monitors_for_mock.assert_has_calls([call(dynamic)])
+        dynamic._octodns['healthcheck']['protocol'] = 'HTTP'
+
+        # Expect to see an update from TCP to HTTP monitor/job_type
+        ## no change if use_http_monitors=False (default)
+        monitors_for_mock.side_effect = [{'1.2.3.4': gend}]
+        extra = provider._extra_changes(desired, [])
+        self.assertFalse(extra)
+        ## change triggered if use_http_monitors=True
+        monitors_for_mock.side_effect = [{'1.2.3.4': gend}]
+        provider.use_http_monitors = True
+        extra = provider._extra_changes(desired, [])
+        self.assertTrue(extra)
+        provider.use_http_monitors = False
 
         # If it's in the changed list, it'll be ignored
         reset()
+        monitors_for_mock.side_effect = [{}]
         extra = provider._extra_changes(desired, [update])
         self.assertFalse(extra)
-        monitors_for_mock.assert_not_called()
+
+        # Missing monitor should trigger an update
+        reset()
+        monitors_for_mock.side_effect = [{}]
+        provider.use_http_monitors = True
+        extra = provider._extra_changes(desired, [])
+        self.assertTrue(extra)
+        provider.use_http_monitors = False
+
+        # Missing monitor for non-obey shouldn't trigger update
+        reset()
+        dynamic.dynamic.pools['iad'].data['values'][0]['status'] = 'up'
+        monitors_for_mock.side_effect = [{}]
+        extra = provider._extra_changes(desired, [])
+        self.assertFalse(extra)
 
         # Test changes in filters
 
         # No change in filters
         reset()
         ns1_zone = {
             'records': [
@@ -2363,14 +2713,15 @@
             ns1_record['type']: ns1_record['filters']
         }
         extra = provider._extra_changes(desired, [])
         self.assertFalse(extra)
 
         # disabled=True in filters does trigger an update
         ns1_zone['records'][0]['filters'][0]['disabled'] = True
+        monitors_for_mock.side_effect = [{}]
         extra = provider._extra_changes(desired, [])
         self.assertTrue(extra)
 
     DESIRED = Zone('unit.tests.', [])
 
     SIMPLE = Record.new(
         DESIRED, 'sim', {'ttl': 33, 'type': 'A', 'value': '1.2.3.4'}
```

